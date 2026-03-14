# Subsets

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1750926302

## Solution Code

```py
class Solution:
    def subsets(self, nums: List[int]) -> List[List[int]]:
        result = [[]] 
        for num in nums:
            newsubsets = []
            for curr in result:
                temp = curr.copy()
                temp.append(num)
                newsubsets.append(temp)
            result.extend(newsubsets) 
        return result
```