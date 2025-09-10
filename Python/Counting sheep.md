### Description 
Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

**Example**
[True,  True,  True,  False,
  True,  True,  True,  True ,
  True,  False, True,  False,
  True,  False, False, True ,
  True,  True,  True,  True ,
  False, False, True,  True] 
  Correct answer would be 17 

  ***Hint*** Don't forget to check for bad values like null/undefined

  ### Solution

  ```Python
def count_sheeps(sheep):
    count = 0
    
    for s in sheep: 
        if s:
            count += 1        
                  
    return count
