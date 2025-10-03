# Description:
Check to see if a string has the same amount of 'x's and 'o's. 

The method must return a boolean and be case insensitive. 

The string can contain any char.

## Examples input/output:

XO("ooxx") => true

XO("xooxx") => false

XO("ooxXm") => true

XO("zpzpzpp") => true // when no 'x' and 'o' is present should return true

XO("zzoo") => false

## Solution 
```python
def xo(s):
    lower_case = s.lower() #converts string to lower case
    x_count = lower_case.count('x') #uses .count to count all x
    o_count = lower_case.count('o')
    
    if x_count == o_count: # if statement to check if the number of xs are equal to numbers of o
        return True
    else: 
        return False
```
