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
```

## Detecting Palindrome word (a word that reads the same backwards)
```python
word = "radar"
if word == word[::-1]:
   print(f"{word} is a plaindrome!")
else:
   print(f"{word} is NOT a plaindrome!")

#word[::-1] - reverses the string
#word == word[::-1] - checks if the original string is the same its reversed
# if its True, then python knows its a palindromne
```
## Detecting palindrome numbers ( a number that repeats) 
```python

n = 12321

if str(n)) == str(n)[::-1]:
   print(f"{n} is a palindrome!")
else:
   print(f"{n} is NOT a palindrome!")
```

## Remove palindrome from a list 
```python

words = ["radar", "level", "hello", "world", "deified"]

non_palindromes = [w for w in words if w != w[::-1]]
print(non_palindromes)
#keeps only words that are NOT palindromes

Output ['hello', 'word']
```
## User input - removing palindromes words dynamically 
```python
user_input = input("enter words: ") #asks for user input
words = user_input.split() #split input into words
non_palindromes = [w for w in words if w !=w[::-1]] # keep only words that are NOT palindromes
cleaned_input = " ".join(non_palindromes) #joins them back into a string

print ("input without palindromes: ", cleaned_input)
```
## User input - removing palindrome numbers dynamically (numbers separated by space)
```python
user_input = input("Enter numbers separated by spaces: ")
numbers =[int(n) for n in user_input.split()] - split input into list of int
non_palindromes = [n for n in numbers if str(n) != str(n)[::-1]] - removes palindromes
print("numbers without palindromes:", non_palindromes)
```
## User input - removing palindrome numbers (single digit) 
```python
user_input = input("Enter numbers: ")
numbers = [int(d) for d in user_input] #- each digit becomes a number 
non_palindromes = [n for n in numbers if str(n) != str(n)[::-1]]
print("Numbers without palindromes:", non_palindromes)




