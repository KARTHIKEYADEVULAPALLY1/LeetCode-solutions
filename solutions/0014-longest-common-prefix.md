# 14. Longest Common Prefix (Easy)

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/longest-common-prefix/description/](https://leetcode.com/problems/longest-common-prefix/description/)
- **Date**: Sep 13, 2026, 9:35 PM
- **Language**: Python

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: 
- Space Complexity: 

Constraints:

1 <= strs.length <= 200
0 <= strs[i].length <= 200
strs[i] consists of only lowercase English letters if it is non-empty.

### 💻 Solution / Code
```python
class Solution:
    def longestCommonPrefix(self, v: List[str]) -> str:
        ans=""
        v=sorted(v)
        first=v[0]
        last=v[-1]
        for i in range(min(len(first),len(last))):
            if(first[i]!=last[i]):
                return ans
            ans+=first[i]
        return ans 

```
