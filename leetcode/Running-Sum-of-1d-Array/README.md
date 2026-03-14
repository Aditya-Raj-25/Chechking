# Running Sum of 1d Array

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1575558026

## Solution Code

```py
class Solution:
    def runningSum(self, nums: List[int]) -> List[int]:
        for i in range(1, len(nums)):
            nums[i] = nums[i] + nums[i - 1]
        return nums
```