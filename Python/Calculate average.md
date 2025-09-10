### Description:
Write a function which calculates the average of the numbers in a given array.

**Note:** Empty arrays should return 0.

```python
def find_average(numbers):
    if len(numbers) == 0: #len function checks if the list if empty
        return 0 #if empty returns 0
    else: 
        return sum(numbers) / len(numbers) #sums the numbers inserted by the user and calculates the average
