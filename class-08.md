# List Comprehensions in Python

**Syntax**

The list comprehension starts with a ‘[‘ and ‘]’, square brackets, to help you remember that the
result is going to be a list.

The basic syntax uses square brackets.

[ expression for item in list if conditional ]
This is equivalent to:

                for item in list:
                    if conditional:
                        expression

Let’s break this down and see what it does.

            ew_list = [expression(i) for i in old_list if filter(i)]
            new_list
            The new list (result).

* expression(i)
Expression is based on the variable used for each element in the old list.


* for i in old_list
The word for followed by the variable name to use, followed by the word in the
old list.

* if filter(i)
Apply a filter with an If-statement.


**new_range = [i * i for i in range(5) if i % 2 == 0]**

Which corresponds to:

*result* = [*transform* *iteration* *filter* ]

The * operator is used to repeat. The filter part answers the question if the
item should be transformed.