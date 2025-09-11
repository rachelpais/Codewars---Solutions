### Slicing cheat sheet

**Example String**
```Python
 s = "hello"
Indexes: 0 1 2 3 4
Chars: h e l l o
```

## Removefirst char
```Python
s[1:] # ello
```

## Remove last character
``` Python
s[:-1] #hell
```

## Remove first and last char
```Python
s[1:-1] #ell
```

## Remove specific index (ex: 2nd char)
```Python
s[:1] + s[2] #hllo
```

## Removing 2 characters 
```Python
s[2:] #llo
```

## Removing last 2 characters
```Python
s[:-2] #hel
```
## Removing 2 characters in the middle (1 & 2) 
```python
s[:1] + s[3:] #hlo
```
## Removing index 0 
```python
s[:0] + s[:1]
```

## Removing 2 consecutive characters starting at index i
```python
s[:i] + s[i+2]
```

## Removing 2 specific characters (h & l) - if the indexes are known
```python
s[:0] + s[1:2] + s[3:] #elo
```

## Using a loop or comprehension (better for multiple or unknown positions) 
```python
s = "hello"
remove_chars = ['h', 'l']
new_s = ''.join([c for c in s if c not in remove_chars])
print(new_s) #eo

#[c for c in s if c not in remove_chars] - goes through each character in s
#''.join(...) - combines it into a string 
```

## Reversing
```python
s[::-1 # olleh
```

## Lists work the same way 
```python
lst = [1,2,3,4,5]
lst[1:-1] # [2,3,4]
lst[::-1] # [5m,4,3,2,1]
lst[:2] + lst[3:] #1,2,,4,5
