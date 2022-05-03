# Class09 Reading Notes

## Reading

[Dunder Methods](https://dbader.org/blog/python-dunder-methods)

These “dunders” or “special methods” in Python are also sometimes called “magic methods.”

Dunder methods let you emulate the behavior of built-in types.

## Object Initialization: \__init__

To construct account objects from the Account class I need a constructor which in Python is the __init__ dunder

## Object Representation: \__str__, \__repr__

\__repr__: The “official” string representation of an object. This is how you would make an object of the class. The goal of \__repr__ is to be unambiguous.

\__str__: The “informal” or nicely printable string representation of an object. This is for the enduser.

## Iteration: \__len__, \__getitem__, \__reversed__

To iterate over transactions in reversed order you can implement the \__reversed__ special method:

## Operator Overloading for Comparing Accounts: \__eq__, \__lt__

## Operator Overloading for Merging Accounts: \__add__

## Callable Python Objects: \__call__
You can make an object callable like a regular function by adding the \__call__ dunder method. 

## Context Manager Support and the With Statement: \__enter__, \__exit__

[Statistics - Probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

normal distribution. The normal distribution refers to a particularly important phenomenon in the realm of probability and statistics.

<a href="https://i.imgur.com/3vDS2Au.png"></a>

The normal distribution is significant to probability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule

Central Limit Theorem
In the previous section, we demonstrated that if we repeated our 10-toss trials many, many times, the average heads-count of all of these trials will approach the 50% we expect from an ideal coin.

Three Sigma Rule
The Three Sigma rule, also known as the empirical rule or 68-95-99.7 rule, is an expression of how many of our observations fall within a certain distance of the mean.

Z-score
The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?”

### Videos

** I didnt really understand the purpose of the videos other than, sometimes people online sound like they know what they are talking about. That may not be the case so you need to be picky about what you accept as true when searching online.

[Intro to Statistics](https://www.youtube.com/watch?v=MdHtK7CWpCQ)

[AI Guru makes $238,800 with misleading paid course. doesn’t credit developers](https://www.youtube.com/watch?v=7jmBE4yPrOs)

### Bookmark and Review

[Statistics Module](https://docs.python.org/3/library/statistics.html)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)