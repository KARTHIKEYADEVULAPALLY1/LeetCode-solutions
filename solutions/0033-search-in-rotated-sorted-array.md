# 0033. Search in Rotated Sorted Array

### 📌 Metadata
- **Source**: [https://leetcode.com/problems/search-in-rotated-sorted-array/description/](https://leetcode.com/problems/search-in-rotated-sorted-array/description/)
- **Difficulty**: Medium
- **Language**: Python
- **Date**: Sep 14, 2026, 12:05 AM

### 💡 Key Takeaways & Intuition
- Intuition: 
- Time Complexity: 
- Space Complexity: 

Constraints:

1 <= nums.length <= 5000
-104 <= nums[i] <= 104
All values of nums are unique.
nums is an ascending array that is possibly rotated.
-104 <= target <= 104

### 💻 Solution / Code
```python
class Solution:
    def search(self, nums: List[int], target: int) -> int:
        left, right = 0, len(nums) - 1
        while left <= right:
            mid = left+(right-left) // 2
            if nums[mid] == target:
                return mid
            if nums[left] <= nums[mid]:
                
                if nums[left] <= target < nums[mid]:
                    right = mid - 1
                else:
                    left = mid + 1
            else:
                if nums[mid] < target <= nums[right]:
                    left = mid + 1
                else:
                    right = mid - 1
        return -1 

```
