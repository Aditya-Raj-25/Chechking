# Valid Parentheses

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1948263644

## Solution Code

```py
class Solution:
    def isValid(self, s: str) -> bool:
        par = {")": "(", "}": "{", "]": "["}
        stack = []
        for c in s:
            if c in par:
                if stack and stack[-1] == par[c]:
                    stack.pop()
                else:
                    return False
            else:
                stack.append(c)
        return True if not stack else False
```