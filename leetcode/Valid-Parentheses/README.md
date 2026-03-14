# Valid Parentheses

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1948276388

## Solution Code

```py
class Solution:
    def isValid(self, s: str) -> bool:
        map = {")": "(", "}": "{", "]": "["}
        stack = []
        for char in s:
            if char in map:
                top_element = stack.pop() if stack else '#'
                if map[char] != top_element: return False
            else: stack.append(char)
        return not stack
```