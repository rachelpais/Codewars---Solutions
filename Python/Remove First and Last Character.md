### Remove First and Last Character
**Task**

The goal is to write a function that removes the first and last characters of a string.

### **Important**

The function should handle strings of any length ≥ 2 characters. For strings with exactly 2 characters, return an empty string.

### **Examples** 

'eloquent' --> 'loquen'
'country'  --> 'ountr' 
'person'   --> 'erso'
'ab'       --> '' (empty string)
'xyz'      --> 'y'

### **Requirements**

The input string will always have at least 2 characters
For strings with exactly 2 characters, return an empty string
For strings with 3 or more characters, remove the first and last character
The function should handle strings containing letters, numbers, and special characters

### Solution
```Python
def remove_char(s):
    return s[1:-1]
```
