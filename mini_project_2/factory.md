# Factory
## Definition
Factory Method is a creational design pattern used to create concrete implementations of a common interface.

It separates the process of creating an object from the code that depends on the interface of the object.

For example, an application requires an object with a specific interface to perform its tasks. The concrete implementation of the interface is identified by some parameter.

Instead of using a complex if/elif/else conditional structure to determine the concrete implementation, the application delegates that decision to a separate component that creates the concrete object. With this approach, the application code is simplified, making it more reusable and easier to maintain.


## Example

```

class MyClass:
	
    def main_one(self, value):  

        if(value == 'A'): definitionA()
	elif(value == 'B'): definitionB()
	else: definitionC()

	def definitionA():
		print("A")
	
	def definitionB():
		print("B")

	def definitionC():
		print("C")

```

**Reference:**
- [https://realpython.com/factory-method-python/](https://realpython.com/factory-method-python/)