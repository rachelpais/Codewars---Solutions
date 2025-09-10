### Description:
Given an array of integers, return a new array with each value doubled.

**For example:**

[1, 2, 3] --> [2, 4, 6]

### Solution 
```python
def maps(a):
    result = [] #creates a new list with each number doubled
    for num in a: 
        result.append(num * 2) 
    return result
