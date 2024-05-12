
Computer Representation of Data

How do we represent raw real world data in a data structure? ==So essentially this lesson is about data structures.==

### Terms
- data matrix - common representation of data, imagine table
- row is a a single observation 
- column is a variable which represents characteristic of each observation
	each variable is of a certain type of data

the library we will use is PANDAS

short for panel data, is a python library designed for analysis of tabular data represented as vectors and matrices. works seamlessly with other data science libraries for python like numpy, matplotlib, scipy.org, scikit learn

### Data Frames
dataframes is the primary pandas data structure, essentially tables 
two dimensional, size mutable potentially heterogenous tabular data.
has unnamed column that we would refer to as the index
contains labeled axes
arithmetic operations align on both row and column labels
can be thought as a dictionary-like container for Series objects
	dictionaries are key-value pairs in python, alike hashmaps in java

### SERIES
- one-dimensional ndarray (numpy) with axis labels
- labels do not need to be unique
- objects supports both integer and level based indexing
- operations between series align values based on their associated index values - not need same length

a dataframe is just a ==combination of multiple series objects==

Applying an operation on a series by a scalar performs the operation on each member of the series
applying an operation on a series and another series performs the operation element wise:
it does operation with matching index
![[Pasted image 20240510150443.png]]



python for data science uses a lot of libraries, python has a built in documentation viewer
just use ? keyword before the function

ex:
`import pandas as pd`
`?pd.read_csv()` - this would show documentation for the function read_csv()

Common Operations
1. view dataset info
	- view dataset info using dataframe.info method (dataframe name)
2. Select Column dataframe["column name"]
	- returns a series object 
3. Select multiple Columns dataframe[["col1", "col2:]]
4. Selecting Row
	- dataframe.loc[index label]
