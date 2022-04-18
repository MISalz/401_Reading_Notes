# Class01 Reading Notes

Reading

[Pain and Suffering](https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering)

This article by CodeFellows is to give you advance notice how hard 401 may be. But just because its hard you need to keep yourself motivated and keep pushing towards the end goal.

[Beginners Guide to Big O ](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/)

#### O(1)
O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

bool IsFirstElementNull(IList\<String> elements)   
\{
    return elements[0] == null;
}

#### O(N)
O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.

bool ContainsValue(IEnumerable\<string> elements, string value)   
\{   
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
}

#### O(N²)
O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. 

bool ContainsDuplicates(IList\<string> elements)   
\{   
    for (var outer = 0; outer < elements.Count; outer++) 
    {   
        for (var inner = 0; inner < elements.Count; inner++)  
        {  
            // Don't compare with self   
            if (outer == inner) continue;  
            if (elements[outer] == elements[inner]) return true;  
        }  
    }    
    return false;
}

#### O(2^N)
O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set.
Additional Resources

int Fibonacci(int number)   
\{
    if (number <= 1) return number;   
    return Fibonacci(number - 2) + Fibonacci(number - 1);  
}

#### Logarithms
This type of algorithm is described as O(log N). The iterative halving of data sets described in the binary search example produces a growth curve that peaks at the beginning and slowly flattens out as the size of the data sets increase e.g. an input data set containing 10 items takes one second to complete, a data set containing 100 items takes two seconds, and a data set containing 1,000 items will take three seconds

[Season 1, Episode 6, A friendly intro to Big O Notation ](https://www.codenewbie.org/basecs/8)



Videos

[Names and Values in Python](https://www.youtube.com/watch?v=_AEJHKGk9ns)


Bookmark and Review

[Awesome Python Environment](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5)

[Python Module of the Week](https://pymotw.com/3/index.html)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)