# 0009. Palindrome Number

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/palindrome-number/](https://leetcode.com/problems/palindrome-number/)
- **Difficulty**: Easy
- **Language**: Python
- **Date**: Sep 13, 2026, 11:58 PM

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: 
- Space Complexity: 

Constraints:

-231 <= x <= 231 - 1

 

Follow up: Could you solve it without converting the integer to a string?

### 💻 Solution / Code
```python
class Solution(object):
    def isPalindrome(self, x):
        if(x<0):
            return False
        rev = 0
        num = x
        while(num>0):
            rev = rev*10 +num%10
            num = num//10
        
        if(rev==x):
            return True
        return False

        

```
