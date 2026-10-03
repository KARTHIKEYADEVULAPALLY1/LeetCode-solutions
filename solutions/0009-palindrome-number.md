# 0009. Palindrome Number

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/palindrome-number/description/](https://leetcode.com/problems/palindrome-number/description/)
- **Difficulty**: Easy
- **Language**: Python
- **Date**: Oct 3, 2026, 1:41 PM

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: O(logx)
- Space Complexity: O(1)

Constraints:

-231 <= x <= 231 - 1

 

Follow up: Could you solve it without converting the integer to a string?

### 💻 Solution / Code
```python
class Solution:
    def isPalindrome(self, x: int) -> bool:
        if x<0:
            return False
        num=x
        rev=0
        while x>0:
            rev=rev*10+x%10
            x=x//10
        if rev==num:
            return True
        return False

```
