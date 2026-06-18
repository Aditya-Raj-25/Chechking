# two sum

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 2037523372

## Solution Code

```py
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        pair_idx = {}

        for i, num in enumerate(nums):
            if target - num in pair_idx:
                return [i, pair_idx[target - num]]
            pair_idx[num] = i

```