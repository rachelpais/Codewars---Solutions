# Description:
You are going to be given a non-empty string. Your job is to return the middle character(s) of the string.

If the string's length is odd, return the middle character.

If the string's length is even, return the middle 2 characters.

## Examples:

"test" --> "es"

"testing" --> "t"

"middle" --> "dd"

"A" --> "A"

## Solution
```python
def get_middle(s):
    length = len(s) # get the length of the string
    
    if length % 2 == 1: #checks if length is odd or even
        middle_index = length // 2
        return s[middle_index] #returns one character using slice
    else: 
        middle_index = length // 2
        return s[middle_index -1 : middle_index +1] #slices the first desired char from the string +1 slices the next char
```
