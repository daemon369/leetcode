# source

	class Solution {
	    public int[] twoSum(int[] nums, int target) {
	        final int[] ret = new int[2];
	        for(int i = 0; i < nums.length-1 ; i++) {
	            final int left = target - nums[i];
	            
	            for(int j = i+1; j < nums.length; j++) {
	                if(nums[j] == left) {
	                    ret[0] = i;
	                    ret[1] = j;
	                    return ret;
	                }
	            }
	        }
	
	        return ret;
	    }
	}

# Runtime

36ms
