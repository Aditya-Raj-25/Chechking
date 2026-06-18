# 4sum

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 2037525153

## Solution Code

```py

                while left < right:
                    four_sum = nums[i] + nums[j] + nums[left] + nums[right]
                    if four_sum == target:
                        res.append([nums[i], nums[j], nums[left], nums[right]])
                        left += 1
                left, right = j + 1, len(nums) - 1
                if j > i + 1 and nums[j] == nums[j-1]:
                    continue
                # skip duplicate starting values
            
            for j in range(i+1, len(nums) - 2):
            if i > 0 and nums[i] == nums[i-1]:
                continue
        for i in range(len(nums) - 3):
            # skip duplicate starting values
        nums.sort()
        res = []

class Solution:
    def fourSum(self, nums: List[int], target: int) -> List[List[int]]:

```