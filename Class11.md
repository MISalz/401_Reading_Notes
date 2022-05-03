# Class11 Reading Notes

### Reading
[What is Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)

Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.

Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

Just read the overview page, what you really want is the video on that page.


[Numpy Tutorial](https://www.dataquest.io/blog/numpy-tutorial-python/)

With NumPy, we work with multidimensional arrays.
A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.

it’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function.

we can use array indexing to select individual elements, groups of elements, or entire rows and columns. One important thing to keep in mind is that just like Python lists, NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0.

: A colon indicates that we want to select all the elements from the starting index up to but not including the ending index. This is also known as a slice

NumPy is a package for working with multidimensional arrays. One of the most common types of multidimensional arrays is the 1-dimensional array, or vector.

NumPy Data Types| type
--|--
float | numeric floating point data.
int | integer data.
string | character data.
object | Python objects.

You can use the numpy.ndarray.astype method to convert an array to a different type.

Single Array Math
If you do any of the basic mathematical operations (/, *, -, +, ^) with an array and a value, it will apply the operation to each of the elements in the array.

Multiple Array Math
It’s also possible to do mathematical operations between arrays. This will apply the operation to pairs of elements. For example, if we add the quality column to itself

Broadcasting involves a few steps:

The last dimension of each array is compared.
If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
Continue checking dimensions until the shortest array is out of dimensions.

NumPy also has several methods that you can use for more complex calculations on arrays. An example of this is the numpy.ndarray.sum method. This finds the sum of all the elements in an array by default:

NumPy makes it possible to test to see if rows match certain values using mathematical comparison operations like <, >, >=, <=, and ==. 

### Videos

Watch the video linked inside What is is Jupyter Lab reading

Bookmark and Review
[Numpy Arrays](https://www.tutorialspoint.com/numpy/index.htm)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)