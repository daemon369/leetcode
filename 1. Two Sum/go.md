# source

	func twoSum(nums []int, target int) []int {
	    l := len(nums)
	
	    var ret [2]int
	    for i:=0;i<l-1;i++ {
	        left := target - nums[i]
	
	        for j:=i+1;j<l;j++ {
	            if nums[j] == left {
	                ret[0] = i
	                ret[1] = j
	                return ret[:]
	            }
	        }
	    }
	
	    return nil
	}

# Runtime

36ms
