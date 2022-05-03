# Class12 Reading Notes

Reading
[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

import pandas as pd

Creating a Series by passing a list of values, letting pandas create a default integer index

Creating a DataFrame by passing a NumPy array, with a datetime index and labeled columns

Creating a DataFrame by passing a dictionary of objects that can be converted into a series-like structure

DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object.

describe() shows a quick statistic summary of your data

pandas primarily uses the value np.nan to represent missing data. 

*Operations in general exclude missing data.*


### Resources


[Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

[Real Python - Pandas Tutorials](https://realpython.com/learning-paths/pandas-data-science/)

### Videos


[What is Pandas](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)

Bookmark and Review
[Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)