## Description:
Complete the function that accepts a string parameter, and reverses each word in the string. All spaces in the string should be retained.

## Examples
"This is an example!" ==> "sihT si na !elpmaxe"

"double  spaces"      ==> "elbuod  secaps"

## Solution

```python 
import re

def reverse_words(text):
    # Splitting the text into words and spaces
    
    parts = re.findall(r'\S+|\s+', text) #uses re.findall() to split the string into pieces. \S+ - matches one or more non space characters. \s+ - matches the spaces 
    
    #Reverse each word, leave spaces as it is 
    
    reversed_parts =[part[::-1] if not part.isspace() else part for part in parts] 
    
    #Joining everything back together
    return ''.join(reversed_parts)
