# 0020. Valid Parentheses

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/valid-parentheses/](https://leetcode.com/problems/valid-parentheses/)
- **Difficulty**: Easy
- **Language**: Python
- **Date**: Sep 14, 2026, 12:02 AM

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: 
- Space Complexity: 

Constraints:

1 <= s.length <= 104
s consists of parentheses only '()[]{}'.

### 💻 Solution / Code
```python
class Solution:
    def isValid(self, s: str) -> bool:
        a=[]
        for i in range(len(s)):
            if s[i]=='('or s[i]=='['or s[i]=='{':
                a.append(s[i])
            else:
                if not a:
                    return False
                top=a.pop()
                if s[i]==')'and top!='(':
                    return False
                if s[i]==']'and top!='[':
                    return False
                if s[i]=='}'and top!='{':
                    return False
        return len(a)==0

            
        

```
