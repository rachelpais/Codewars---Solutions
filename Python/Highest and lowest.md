# Description:
In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.

## Examples
high_and_low("1 2 3 4 5") # return "5 1"
high_and_low("1 2 -3 4 5") # return "5 -3"
high_and_low("1 9 3 4 -5") # return "9 -5"

## Notes
All numbers are valid Int32, no need to validate them.
There will always be at least one number in the input string.
Output string must be two numbers separated by a single space, and highest number is first.

## Solution

```python
def high_and_low(numbers):
    
    num_list = [int(n) for n in numbers.split()] #splits the string into individual ints
    highest = max(num_list) #stores the highest number
    lowest = min(num_list) #stores the lowest number
    
    return str(highest) + " " + str(lowest) #returns ints back as strings
```
