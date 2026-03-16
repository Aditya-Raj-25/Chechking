# Search Insert Position

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1949725624

## Solution Code

```py
class Solution:
    def searchInsert(self, nums: List[int], target: int) -> int:
        left, right = 0, len(nums) - 1
        while left <= right:
            mid = (left + right) // 2
            if nums[mid] == target:
                return mid
            elif nums[mid] < target:
                left = mid + 1
            else:
                right = mid - 1
        return left
```