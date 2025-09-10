## Grasshopper - Personalized Message

### Description
Create a function that gives a personalized greeting. This function takes two parameters: `name` and `owner`.

Use conditionals to return the proper message:

| Case            | Return         |
|-----------------|----------------|
| name equals owner | "Hello boss"  |
| otherwise        | "Hello guest" |

### Solution 
```python
def greet(name, owner):
    if name == owner:
        return "Hello boss"
    else:
        return "Hello guest"
