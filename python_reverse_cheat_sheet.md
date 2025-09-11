### ------------------------------------------------------------------------------------- 
###                                     Python Reverse Cheat sheet                                  
### -------------------------------------------------------------------------------------

# Reversing int

``` Python
def reverse_int(n):
    return [int(c) for c in str(n)][::-1]
# 1.As python reads the int as a single value, the int must be converted to a string str(n) - accesses individual digits
# 2.As Python cannot sum strings, it needs to be converted back to int int(c)
# 3.The reversal happens after the characters are reverted back to int using [::-1]
```
# Reversing a list 
``` Python
numbers = [1,2,3,4,5]
print(numbers[::-1]) # [5,4,3,2,1]

colours = ["red", "green", "blue"]
print(colours[::-1]) #blue, green, red
```

# Reversing a string 
```Python
word = "hello"
print(word[::-1]) #olleh
```

# Reversing a tuple 
```Python
t = (1,2,3)
print(t[::-1])
```

# Reversing a range - must be converted to a list first
```Python
r  = range(5)
print(list(r)[::-1])
```

# Reversing the whole dictionary (items)
```Python
my_dict = {"a": 1, "b": 2, "c": 3}

# Reverse order of key-value pairs
reversed_dict = dict(reversed(list(my_dict.items())))
print(reversed_dict)  # {'c': 3, 'b': 2, 'a': 1}
```

# Reversing only keys or values
``` Python
# Reverse only keys
reversed_keys = list(my_dict.keys())[::-1]
print(reversed_keys)  # ['c', 'b', 'a']

# Reverse only values
reversed_values = list(my_dict.values())[::-1]
print(reversed_values)  # [3, 2, 1]
```





    
