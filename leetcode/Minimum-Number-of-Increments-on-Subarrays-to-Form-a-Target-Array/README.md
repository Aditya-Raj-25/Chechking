# Minimum Number of Increments on Subarrays to Form a Target Array

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1782009119

## Solution Code

```py
class Solution:
    def minNumberOperations(self, target: List[int]) -> int:
        operations=target[0]
        for i in range(1,len(target)):
            if target[i]>target[i-1]:
                operations+=target[i]-target[i-1]
        return operations
```