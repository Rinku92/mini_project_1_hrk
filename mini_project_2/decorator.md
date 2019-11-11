# Decorator
## Definition
In Decorators, functions are taken as the argument into another function and then called inside the wrapper function.

Decorators are very powerful and useful tool in Python since it allows programmers to modify the behavior of function or class. Decorators allow us to wrap another function in order to extend the behavior of wrapped function, without permanently modifying it.


## Example

```

def decorator_A(func_B):
	def func_C():
		func_B()
		return func_C

def the_main_one():
	the_main_one = decorator_A(the_main_one)

the_main_one()
```

**Reference:**
- [https://www.geeksforgeeks.org/decorators-in-python/](https://www.geeksforgeeks.org/decorators-in-python/)