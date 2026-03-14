# Complement of Base 10 Integer

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1944951275

## Solution Code

```py
class Solution:
    def bitwiseComplement(self, n: int) -> int:
        if n == 0:
            return 1
        mask = 1
        while mask <= n:
            mask <<= 1
        return (mask - 1) ^ n
```