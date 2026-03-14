# Binary Tree Inorder Traversal

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1734546146

## Solution Code

```py
# Definition for a binary tree node.
# class TreeNode:
#     def __init__(self, val=0, left=None, right=None):
#         self.val = val
#         self.left = left
#         self.right = right
class Solution:
    def inorderTraversal(self, root: Optional[TreeNode]) -> List[int]:
        if not root:
            return []
        return self.inorderTraversal(root.left)+[root.val]+self.inorderTraversal(root.right)
```