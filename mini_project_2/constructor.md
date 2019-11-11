# Constructor
## Definition
Constructors are generally used for instantiating an object.The task of constructors is to initialize(assign values) to the data members of the class when an object of class is created.In Python the __init__() method is called the constructor and is always called when an object is created.

## Syntax

```
def __init__(self):
    # body of the constructor
```

## Example

```

class MyClass:
	
	a = 6
    def __init__(self, i):  #constructor
        self.a = i

```

**Reference:**
- [https://www.geeksforgeeks.org/constructors-in-python/](https://www.geeksforgeeks.org/constructors-in-python/)