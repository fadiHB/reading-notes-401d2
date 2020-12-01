## Python Classes/Objects

Python is an object oriented programming language.

Almost everything in Python is an object, with its properties and methods.

A Class is like an object constructor, or a "blueprint" for creating objects.

### The __init__() Function
The examples above are classes and objects in their simplest form, and are not really useful in real life applications.

To understand the meaning of classes we have to understand the built-in __init__() function.

All classes have a function called __init__(), which is always executed when the class is being initiated.

Use the __init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created:


### Object Methods
Objects can also contain methods. Methods in objects are functions that belong to the object.

### The self Parameter
The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:


### Delete Object Properties
You can delete properties on objects by using the del keyword:


### Delete Objects
You can delete objects by using the del keyword:

### The pass Statement
class definitions cannot be empty, but if you for some reason have a class definition with no content, put in the pass statement to avoid getting an error.

## Thinking Recursively in Python

![img](https://files.realpython.com/media/Thinking-Recursively-in-Python_Watermarked.1825397c00ea.jpg)


### Maintaining State

When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

* Thread the state through each recursive call so that the current state is part of the current call’s execution context
* Keep the state in global scope


### Pesky Details

Python doesn’t have support for tail-call elimination. As a result, you can cause a stack overflow if you end up using more stack frames than the default call stack depth:

                            >>> import sys
                            >>> sys.getrecursionlimit()
                            3000
Keep this limitation in mind if you have a program that requires deep recursion.

Also, Python’s mutable data structures don’t support structural sharing, so treating them like immutable data structures is going to negatively affect your space and GC (garbage collection) efficiency because you are going to end up unnecessarily copying a lot of mutable objects. For example, I have used this pattern to decompose lists and recurse over them:

                                >>> input_list = [1, 2, 3]
                                >>> head = input_list[0]
                                >>> tail = input_list[1:]
                                >>> print("head --", head)
                                head -- 1
                                >>> print("tail --", tail)
                                tail -- [2, 3]
I did that to simplify things for the sake of clarity. Keep in mind that tail is being created by copying. Recursively doing that over large lists can negatively affect your space and GC efficiency.


## Testing Python Applications with Pytest

Testing applications has become a standard skill set required for any competent developer today. The Python community embraces testing, and even the Python standard library has good inbuilt tools to support testing. In the larger Python ecosystem, there are a lot of testing tools. Pytest stands out among them due to its ease of use and its ability to handle increasingly complex testing needs.


## pytest fixtures: explicit, modular, scalable
Software test fixtures initialize test functions. They provide a fixed baseline so that tests execute reliably and produce consistent, repeatable, results. Initialization may setup services, state, or other operating environments. These are accessed by test functions through arguments; for each fixture used by a test function there is typically a parameter (named after the fixture) in the test function’s definition.

