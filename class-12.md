# Pandas

## how to imoptant
 import pandas as pd


## DataFrame

 class pandas.DataFrame(data=None, index=None, columns=None, dtype=None, copy=False)[source]
Two-dimensional, size-mutable, potentially heterogeneous tabular data.

Data structure also contains labeled axes (rows and columns). Arithmetic operations align on both row and column labels. Can be thought of as a dict-like container for Series objects. The primary pandas data structure.

Parameters
**data** ndarray (structured or homogeneous), Iterable, dict, or DataFrame
Dict can contain Series, arrays, constants, or list-like objects.

Changed in version 0.23.0: If data is a dict, column order follows insertion-order for Python 3.6 and later.

Changed in version 0.25.0: If data is a list of dicts, column order follows insertion-order for Python 3.6 and later.

**index** : Index or array-like
Index to use for resulting frame. Will default to RangeIndex if no indexing information part of input data and no index provided.

**columns** : Index or array-like
Column labels to use for resulting frame. Will default to RangeIndex (0, 1, 2, …, n) if no column labels are provided.

**dtype** : dtype, default None
Data type to force. Only a single dtype is allowed. If None, infer.

**copy** : bool, default False
Copy data from inputs. Only affects DataFrame / 2d ndarray input.

## Series

Series is a one-dimensional labeled array capable of holding any data type (integers, strings, floating point numbers, Python objects, etc.). The axis labels are collectively referred to as the index. The basic method to create a Series is to call:

>>> s = pd.Series(data, index=index)
Here, data can be many different things:

* a Python dict

* an ndarray

* a scalar value (like 5)


## Grouping

By “group by” we are referring to a process involving one or more of the following steps:

+ Splitting the data into groups based on some criteria

+ Applying a function to each group independently

+ Combining the results into a data structure

## Pivot tables

While pivot() provides general purpose pivoting with various data types (strings, numerics, etc.), pandas also provides pivot_table() for pivoting with aggregation of numeric data.

The function pivot_table() can be used to create spreadsheet-style pivot tables. See the cookbook for some advanced strategies.

It takes a number of arguments:

**data**: a DataFrame object.

**values**: a column or a list of columns to aggregate.

**index**: a column, Grouper, array which has the same length as data, or list of them. Keys to group by on the pivot table index. If an array is passed, it is being used as the same manner as column values.

**columns**: a column, Grouper, array which has the same length as data, or list of them. Keys to group by on the pivot table column. If an array is passed, it is being used as the same manner as column values.

**aggfunc**: function to use for aggregation, defaulting to numpy.mean.

## Time series / date functionality¶

pandas contains extensive capabilities and features for working with time series data for all domains. Using the NumPy datetime64 and timedelta64 dtypes, pandas has consolidated a large number of features from other Python libraries like scikits.timeseries as well as created a tremendous amount of new functionality for manipulating time series data.

## Categorical data¶

This is an introduction to pandas categorical data type, including a short comparison with R’s factor.

Categoricals are a pandas data type corresponding to categorical variables in statistics. A categorical variable takes on a limited, and usually fixed, number of possible values (categories; levels in R). Examples are gender, social class, blood type, country affiliation, observation time or rating via Likert scales.

In contrast to statistical categorical variables, categorical data might have an order (e.g. ‘strongly agree’ vs ‘agree’ or ‘first observation’ vs. ‘second observation’), but numerical operations (additions, divisions, …) are not possible.

All values of categorical data are either in categories or np.nan. Order is defined by the order of categories, not lexical order of the values. Internally, the data structure consists of a categories array and an integer array of codes which point to the real value in the categories array.

The categorical data type is useful in the following cases:

* A string variable consisting of only a few different values. Converting such a string variable to a categorical variable will save some memory, see here.

* The lexical order of a variable is not the same as the logical order (“one”, “two”, “three”). By converting to a categorical and specifying an order on the categories, sorting and min/max will use the logical order instead of the lexical order, see here.

* As a signal to other Python libraries that this column should be treated as a categorical variable (e.g. to use suitable statistical methods or plot types).
