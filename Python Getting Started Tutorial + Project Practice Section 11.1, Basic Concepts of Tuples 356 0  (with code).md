directory 

11.1.1 understand tuple types 

Type name of 11.1.2 tuple 

Definition of 11.1.3 tuple 

11.1.4 unpacking of tuples 

11.1.5 Traverse Iterable Objects 

11.1.6 Knowledge points in this section 

Learn Python 11.1.7 System 

##  11.1.1 understand tuple types 

Tuples have the same data structure as lists, except that tuples are static data types, while lists are dynamic data types. The differences between tuples and lists are explained in detail in Section 11.4. The tuple type in Python is a set of data enclosed by the () symbol, and the elements in the set are separated by commas. Like lists, tuples can contain any data type: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
![avatar]( 922a41b52acf9ff7b468765142711036.png) 

Tuples, like lists and strings, are a linear sequential table structure. 

![avatar]( cb17f02bb5eb01f87c08bb03dd9e0f7f.png) 

>  Students who are not familiar with linear sequential table structures can review the content of Section 9.1, "Basic Concepts of Strings". 

In a linear sequence structure, elements in a data set can be accessed by indexing: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
Indexes in Python are numbered from 0, 0 for the first position, and 1 for the second position. Python also supports negative indices, which are numbered from -1, -1 for the penultimate position, -2 for the penultimate position, and so on. 

##  Type name of 11.1.2 tuple 

In interactive mode, type to output the type name of a string: 

>  >>> container = (1, '2', 3.0, True)

> >> type(container)

<class 'tuple'> 

From the output, the type of the tuple is named tuple. 

##  Definition of 11.1.3 tuple 

The definition of tuples mainly includes object definition method and direct definition method. 

(1) Object definition method 

The type name of the tuple is tuple. You can directly execute help (tuple) in interactive mode to find the definition and usage of tuple: 

>  class tuple(object)

|  tuple(iterable=(), /)

|

|  Built-in immutable sequence.

|

|  If no argument is given, the constructor returns an empty tuple.

|  If iterable is specified the tuple is initialized from iterable's items.

|

|  If the argument is a tuple, the return value is the same object. 

In the output of the interactive mode, the form of tuple (iterable = (),/) is the object definition method. The parameter iterable represents an iterable object. Among the data types learned so far, string, list, and tuple are all iterable objects. In Python, any data type that can traverse the elements in the collection is an iterable object. The so-called traversal is to access the elements in the collection one by one. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
(2) Direct definition method 

The so-called direct definition method is to define tuples directly through the () symbol: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
List types can contain any data type, and now nested tuples are defined by direct definition. The so-called nested tuple refers to the inclusion of tuples in tuples. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
When defining a tuple, you can also directly remove (), and Python will automatically treat a comma-separated element as a tuple. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
##  10.1.4 unpacking of tuples 

When assigning a tuple to another variable, Python automatically unpacks the tuple. To understand the concept of unpacking, let's take a look at a simple code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
Code explanation: 

>  (1) Tuple unpacking is to disassemble the tuple and then assign the elements in the tuple in sequence

(2) In the code a, b, c = container, assign the elements of the tuple container to the variables on the left in order 

When unpacking a tuple, the number of variables on the left side of the assignment operator must match the number of elements in the tuple, otherwise an exception will be thrown. 

How to unpack a tuple when there is only one element? 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
##  11.1.4 Traverse Iterable Objects 

The simple data types in Python are all non-iterable objects. The simple data types learned so far are integers, floating-point types, and boolean types. Composite data types in Python are all iterable objects. For iterable objects, you can iterate over the elements in the collection in the for loop structure. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532615
 ```  
##  11.1.5 Knowledge points in this section 

>  (1) A tuple type is a collection of data that arranges the elements in the collection in order

(2) In Python, the tuple type is surrounded by (), and the elements in () are separated by English commas

(3) The type name of a tuple is tuple. Like strings and lists, tuples are also linear sequence structures

(4) Tuples can be defined by object definition and direct definition

(5) Simple data types are non-iterable, and composite data types in Python are all iterable objects

(6) For iterable objects, you can iterate through the elements in the collection in a for loop 

##  Learn Python 11.1.6 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

