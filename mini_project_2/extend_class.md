# Extend Class
## Definition
Inheritance allows programmers to create classes that are built upon existing classes, and this makes it possible that a class created through inheritance inherites the attributes and methods of the parent class. This means that inheritance supports code reusability. The methods or generally speaking the software inherited by a subclass is considered to be reused in the subclass. The relationships of objects or classes through inheritance give rise to a directed graph.

The class from which a class inherits is called the parent or superclass. A class which inherits from a superclass is called a subclass, also called heir class or child class. Superclasses are sometimes called ancestors as well. There exists a hierarchy relationship between classes

## Syntax

```
class DerivedClassName(BaseClassName):
    pass
```

## Example

```

class Car:
    
    def __init__(self, name):
        self.name = name
        
    def say_hello(self):
        print("Hello, I am " + self.name)
        
class Tesla(Car):
    def __init__(self, name):
        super.__init__.name = name

```

**Reference:**
- [https://www.python-course.eu/python3_inheritance.php](https://www.python-course.eu/python3_inheritance.php)