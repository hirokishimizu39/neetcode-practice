# Contains Duplicate

LeetCode: [217](https://leetcode.com/problems/contains-duplicate/)
Difficulty: Easy
Category: Arrays & Hashing

## Problem Description

Given an integer array `nums`, return `true` if any value appears at least twice in the array, and return `false` if every element is distinct.

## Interview Framework

### 1. Input
- `nums`: integer array
- Constraints: 1 <= nums.length <= 10^5, -10^9 <= nums[i] <= 10^9

### 2. Output
- `boolean`: true if duplicates exist, false otherwise

### 3. Basic Idea
- Use HashSet to track seen numbers
- O(1) lookup for each element
- First duplicate found → return true

### 4. Implementation Ideas
1. Initialize empty HashSet
2. Iterate through array
3. For each element: check if in set → return true, else add to set
4. Return false after loop

### 5. Edge Cases
- [x] Single element → false
- [x] All same elements → true
- [x] All unique elements → false
- [x] Two elements, same → true

---

## Solutions

### C++ Solution

```cpp
// Time: O(n)
// Space: O(n)
class Solution {
public:
    bool containsDuplicate(vector<int>& nums) {
        unordered_set<int> seen;
        for (int num : nums) {
            if (seen.count(num)) return true;
            seen.insert(num);
        }
        return false;
    }
};
```

### Python Solution

```python
# Time: O(n)
# Space: O(n)
class Solution:
    def containsDuplicate(self, nums: list[int]) -> bool:
        seen = set()
        for num in nums:
            if num in seen:
                return True
            seen.add(num)
        return False
```

### TypeScript Solution

```typescript
// Time: O(n)
// Space: O(n)
function containsDuplicate(nums: number[]): boolean {
    const seen = new Set<number>();
    for (const num of nums) {
        if (seen.has(num)) return true;
        seen.add(num);
    }
    return false;
}
```

### Go Solution

```go
// Time: O(n)
// Space: O(n)
func containsDuplicate(nums []int) bool {
    seen := make(map[int]bool)
    for _, num := range nums {
        if seen[num] {
            return true
        }
        seen[num] = true
    }
    return false
}
```

---

## Learning Notes

### Key Insights
- HashSet provides O(1) average lookup
- Early return optimization

### Mistakes Made
-

### Related Problems
- 219: Contains Duplicate II
- 220: Contains Duplicate III

### Review Count
| Date | Language | Time | Passed |
|------|----------|------|--------|
| | | | |
