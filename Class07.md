# Class07 Reading Notes

Reading
NOTE This is a long reading. The portion to make sure you cover is on global and nonlocal keywords. You can skim the rest.

[Python Scope](https://realpython.com/python-scope-legb-rule/)

Scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope. 

|Operation|	Statement|
--|--
Assignments	| x = value
Import operations	| import module or from module import name
Function definitions |	def my_func(): ...
Argument definitions | in the context of functions	def my_func(arg1, arg2,... argN): ...
Class definitions |	class MyClass: ...

**Global scope:** The names that you define in this scope are available to all your code.

**Local scope:** The names that you define in this scope are only available or visible to the code within the scope.

**Note:** There’s an important difference between assignment operations and reference or access operations. When you reference a name, you’re just retrieving its content or value. When you assign a name, you’re either creating that name or modifying it.

Python scopes are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces. 

They’re stored in a special attribute called .\__dict__.

After you import sys, you can use .keys() to inspect the keys of sys.\__dict__. This returns a list with all the names defined at the top level of the module. I

Videos
NOTE* The repeated Big O content is intentional. This is a big concept and worth hearing about from multiple presenters. TIP: watch on faster speed if you like.

## LEGB rule

**Local (or function)** scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

**Enclosing (or nonlocal)** scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

**Global (or module)** scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

**Built-in** scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.


[Don’t be CONFUSED by BIG O notation anymore!](https://www.youtube.com/watch?v=5Uqawfl0VHQ)

Bookmark and Review
[Rolling Dice Examples](https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)