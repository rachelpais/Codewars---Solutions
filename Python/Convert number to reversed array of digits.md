### Description:
Given a random non-negative number, you have to return the digits of this number within an array in reverse order.

**Example (Input => Output):**
35231 => [1,3,2,5,3]
0     => [0]

### Solution 
```Python
def digitize(n):
    return [int(c) for c in str(n)][::-1] 
#converted the number n to a string so that Python can access every digit
#converted each character back into an int 
#Reversed the list using [::-1] 
