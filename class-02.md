
## Test in python
### What is TDD and why is it important?

![GitHub Logo](https://www.xenonstack.com/images/blog/Test-Driven-Development-Python.png)

In layman’s terms, TDD recommends writing tests that would check the functionality of your code prior to your writing the actual code. Only when you are happy with your tests and the features it tests, do you begin to write the actual code in order to satisfy the conditions imposed by the test that would allow them to pass.

### Unit tests and TDD?

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

### What is PyTest?

Pytest is a testing framework which allows us to write test codes using python. You can write code to test anything like database , API, even UI if you want. But pytest is mainly being used in industry to write tests for APIs.

#### Why use PyTest?

Some of the advantages of pytest are

* Very easy to start with because of its simple and easy syntax.
* Can run tests in parallel.
* Can run a specific test or a subset of tests
* Automatically detect tests
* Skip tests
* Open source

## What is Recursion? 

The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. 


## Python Lists

Python has a great built-in list type named "list". List literals are written within square brackets [ ]. Lists work similarly to strings -- use the len() function and square brackets [ ] to access data, with the first element at index 0

**FOR and IN**
Python's *for* and *in* constructs are extremely useful, and the first use of them we'll see is with lists. The *for* construct -- for var in list -- is an easy way to look at each element in a list (or other collection). Do not add or remove from the list during iteration.

## While Loop

Python also has the standard while-loop, and the *break* and *continue* statements work as in C++ and Java, altering the course of the innermost loop. The above for/in loops solves the common case of iterating over every element in a list, but the while loop gives you total control over the index numbers. Here's a while loop which accesses every 3rd element in a list:

## List Methods
Here are some other common list methods.

* list.append(elem) -- adds a single element to the end of the list. Common error: does not return the new list, just modifies the original.
* list.insert(index, elem) -- inserts the element at the given index, shifting elements to the right.
* list.extend(list2) adds the elements in list2 to the end of the list. Using + or += on a list is similar to using extend().
* list.index(elem) -- searches for the given element from the start of the list and returns its index. Throws a ValueError if the element does not appear (use "in" to check without a ValueError).
* list.remove(elem) -- searches for the first instance of the given element and removes it (throws ValueError if not present)
* list.sort() -- sorts the list in place (does not return it). (The sorted() function shown later is preferred.)
* list.reverse() -- reverses the list in place (does not return it)
* list.pop(index) -- removes and returns the element at the given index. Returns the rightmost element if index is omitted (roughly the opposite of append()).

## String Methods
Here are some of the most common string methods. A method is like a function, but it runs "on" an object. If the variable s is a string, then the code s.lower() runs the lower() method on that string object and returns the result (this idea of a method running on an object is one of the basic ideas that make up Object Oriented Programming, OOP). Here are some of the most common string methods:

* s.lower(), s.upper() -- returns the lowercase or uppercase version of the string
* s.strip() -- returns a string with whitespace removed from the start and end
* s.isalpha()/s.isdigit()/s.isspace()... -- tests if all the string chars are in the various character classes
* s.startswith('other'), s.endswith('other') -- tests if the string starts or ends with the given other string
* s.find('other') -- searches for the given other string (not a regular expression) within s, and returns the first index where it begins or -1 if not found
* s.replace('old', 'new') -- returns a string where all occurrences of 'old' have been replaced by 'new'
* s.split('delim') -- returns a list of substrings separated by the given delimiter. The delimiter is not a regular expression, it's just text. 'aaa,bbb,ccc'.split(',') -> ['aaa', 'bbb', 'ccc']. As a convenient special case s.split() (with no arguments) splits on all whitespace chars.
* s.join(list) -- opposite of split(), joins the elements in the given list together using the string as the delimiter. e.g. '---'.join(['aaa', 'bbb', 'ccc']) -> aaa---bbb---ccc