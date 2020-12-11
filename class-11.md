# Class 11

## JupyterLab

is a next-generation web-based user interface for Project Jupyter.

JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner

You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:

* **Code Consoles** provide transient scratchpads for running code interactively, with full support for rich output
* **Kernel-backed documents** enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.
* Notebook cell outputs can be **mirrored into their own tab**, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.
* Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers

## NumPy

NumPy is an open source project aiming to enable numerical computing with Python.
It was created in 2005, building on the early work of the Numerical and Numarray libraries.
NumPy will always be 100% open source software, free for all to use and released under the liberal terms of the modified BSD license.

### Numpy 2-Dimensional Arrays

Arrays that require two subscripts to identify a particular element are called two-dimensional arrays or 2-D arrays,also known as a matrix

### NumPy To Read In Files

It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. We can use it to read in our initial data on red wines.

## Indexing NumPy Arrays

We can use array indexing to select individual elements, groups of elements, or entire rows and columns.

## NumPy Array Methods

In addition to the common mathematical operations, NumPy also has several methods that you can use for more complex calculations on arrays.
e.g

* numpy.ndarray.mean — finds the mean of an array.
* numpy.ndarray.std — finds the standard deviation of an array.
* numpy.ndarray.min — finds the minimum value in an array.
* numpy.ndarray.max — finds the maximum value in an array.

## NumPy Array Operations

NumPy makes it simple to perform mathematical operations on arrays. This is one of the primary advantages of NumPy, and makes it quite easy to do computations.

* Single Array Math
If you do any of the basic mathematical operations (/, *, -, +, ^) with an array and a value, it will apply the operation to each of the elements in the array.

* Multiple Array Math
It’s also possible to do mathematical operations between arrays. This will apply the operation to pairs of elements.

* Broadcasting
Unless the arrays that you’re operating on are the exact same size, it’s not possible to do elementwise operations. In cases like this, NumPy performs broadcasting to try to match up elements. Essentially, broadcasting involves a few steps:

+ The last dimension of each array is compared.
    + If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
    + If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
+ Continue checking dimensions until the shortest array is out of dimensions.


## NumPy Array Methods

In addition to the common mathematical operations, NumPy also has several methods that you can use for more complex calculations on arrays.
e.g:

* ndarry()
* sum()
* deg2rad()
* rad2deg()

## Reshaping NumPy Arrays

We can change the shape of arrays while still preserving all of their elements. This often can make it easier to access array elements.
some usuful function :

* numpy.transpose function:
* numpy.ravel function 
* numpy.reshape function

### Importing the library

**import** numpuy as **np**
