## Opposties Attract Kata 

Timmy & Sarah think they are in love, but in their town, they will only know once they each pick a flower.  

**Rule:**  
- If one flower has an **even number of petals** and the other has an **odd number of petals**, it means they are in love.  

### Task
Write a function that takes the number of petal of each flower as input and returns: 
- 'True' if they are in love
- 'False' if they are not 

### Examples
lovefunc(1, 4) # True
lovefunc(2, 2) # False
lovefunc(0, 1) # True
lovefunc(0, 0) # False

### Solution 
```python
def lovefunc(flower1, flower2):  # Flower 1 = Timmy, Flower 2 = Sarah
    # checks if both flowers are odd or even and compares results
    if (flower1 % 2) != (flower2 % 2):
        return True
    else:
        return False

