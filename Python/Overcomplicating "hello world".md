### Description:
Make a simple function called greet that returns the most-famous "hello world!".

### Style Points
Sure, this is about as easy as it gets. But how clever can you be to create the most creative "hello world" you can think of? What is a "hello world" solution you would want to show your friends?

### Solution 
``` Python 
def greet():
    
    letters = ["h", "e", "l", "l", "o", " ", "w", "o", "r", "l", "d", "!"]                      
    
    message = "".join(letters) #joins them back into a string
    
    return message.lower()#ensures return is in lowercase
