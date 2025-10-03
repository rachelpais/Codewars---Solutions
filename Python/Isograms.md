# Description:
An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

## Example: (Input --> Output) 

```
"Dermatoglyphics" --> true
"aba" --> false
"moOse" --> false (ignore letter case)
```

## Solution 
```python
def is_isogram(string):
    
    string = string.lower() #converts the input string to lowercase 
    seen_letters = set() #creates an empty set 

    for letter in string: 
        if letter in seen_letters:
            return False
        seen_letters.add(letter)
            
    return True
```

