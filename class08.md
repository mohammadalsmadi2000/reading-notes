# Class 08

## List Comprehensions:

List comprehension is a concise way of creating a list in Python. It consists of an expression followed by a for clause and zero or more if clauses. The basic syntax of Python list comprehension is:

```
new_list = [expression for item in iterable if condition]

```
This creates a new list called new_list by iterating over an existing iterable and applying the expression to each element that meets the condition (if provided).

The same list can be created using a for loop as follows:
```
old_list = [1, 2, 3, 4, 5]
new_list = []
for item in old_list:
    if item > 2:
        new_list.append(item ** 2)

```
The list comprehension for the above example would be:

```
old_list = [1, 2, 3, 4, 5]
new_list = [item ** 2 for item in old_list if item > 2]

```

This creates a new list called new_list by iterating over old_list and squaring each element that is greater than 2.

## Decorators in Python:
In Python, a decorator is a special type of function that takes another function as input and extends the behavior of the input function without modifying its code. The basic syntax of a decorator function is:

```
def decorator_function(original_function):
    def wrapper_function(*args, **kwargs):
        # do something before the original function is called
        result = original_function(*args, **kwargs)
        # do something after the original function is called
        return result
    return wrapper_function

```

The decorator function takes an original function as input and returns a wrapper function that adds some functionality before and/or after the original function is called. To use the decorator, we can simply apply it to the original function using the @ symbol:

```
@decorator_function
def original_function(*args, **kwargs):
    # do something

```
This replaces the original function with the wrapper function that has the extended behavior.

Decorators are commonly used in Python for tasks such as logging, timing, caching, and authentication.

Example of a simple decorator function from the reading:
```
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()

```

The above code applies the my_decorator function to the say_hello function using the @ symbol. When say_hello is called, it first prints a message before calling the original function, and then prints another message after the function is called.
