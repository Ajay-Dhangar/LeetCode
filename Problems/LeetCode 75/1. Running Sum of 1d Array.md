### 1480. Running Sum of 1d Array

[Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/?envType=study-plan&id=level-1)

**Solution in Java**

```
class Solution {
    public int[] runningSum(int[] nums) {
        int n = nums.length;  // size of array
        for(int i=1; i<n; i++){    
            nums[i] = nums[i-1] + nums[i];  // logic [1, 1+2, 1+2+3, 1+2+3+4].
        }
        return nums; // return array
    }
}
```