# source

	/**
	* Note: The returned array must be malloced, assume caller calls free().
	*/
	int* twoSum(int* nums, int numsSize, int target) {
	  int i, j, index;
	  int left = 0;
	  int* ret;
	  ret = malloc(sizeof(int)*2);
	  for(i=0;i<numsSize-1;i++) {
	      left = target - nums[i];
	
	      for(j=i+1;j<numsSize;j++) {
	          if(left == nums[j]) {
	              ret[0] = i;
	              ret[1] = j;
	              return ret;
	          }
	      }
	  }
	
	  return NULL;
	}

# Runtime

56ms
