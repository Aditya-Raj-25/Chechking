# Remove Element

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1948383617

## Solution Code

```py
class Solution:
    def removeElement(self, nums: List[int], val: int) -> int:
        k = 0
        for i in range(len(nums)):
            if nums[i] != val:
                nums[k] = nums[i]
                k += 1
        return k
```