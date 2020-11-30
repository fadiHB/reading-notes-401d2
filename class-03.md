
## Reading and Writing Files in Python

### What Is a File?

At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file

#### File Paths

When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. File Name: the actual name of the file
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

### Opening and Closing a File in Python

When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:

after that .should close the file ..

best way to do theses thing together is ...

                        with open('dog_breeds.txt') as reader:
                            # Further file processing goes here

| :---: | :---: |
| Character | Meaning |
| 'r' | Open for reading (default) |
| 'w' | Open for writing, truncating (overwriting) the file first |
| 'rb' or 'wb' | Open in binary mode (read/write using byte data) |

## Python Exceptions: An Introduction

### Exceptions versus Syntax Errors

Syntax errors occur when the parser detects an incorrect statement. 

### Raising an Exception

We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

### The AssertionError Exception

Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

### The try and except Block: Handling Exceptions

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

### The else Clause

In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

### Cleaning Up After Using finally

Imagine that you always had to implement some sort of action to clean up after executing your code. Python enables you to do so using the finally clause.

[class3](img/class3.PNG)
