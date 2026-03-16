# Length of Last Word

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1949726721

## Solution Code

```py
class Solution:
    def lengthOfLastWord(self, s: str) -> int:
        return len(s.strip().split()[-1])
```