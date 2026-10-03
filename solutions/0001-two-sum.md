# 0001. Two Sum

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/two-sum/](https://leetcode.com/problems/two-sum/)
- **Difficulty**: Easy
- **Language**: Python
- **Date**: Oct 3, 2026, 1:06 PM

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: O(N^2)
- Space Complexity:O(1) 

Constraints:

2 <= nums.length <= 104
-109 <= nums[i] <= 109
-109 <= target <= 109
Only one valid answer exists.

 

Follow-up: Can you come up with an algorithm that is less than O(n2) time complexity?

### 💻 Solution / Code
```python
class Solution:
    def twoSum(self, nums: list[int], target: int) -> list[int]:
        for i in range(len(nums)):
            for j in range(1,len(nums)):
                if nums[i]+nums[j]==target:
                    return [i,j]

```
