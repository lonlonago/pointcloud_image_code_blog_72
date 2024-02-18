directory 

11.4.1 Immutable Data Types 

11.4.2 Variable Data Types 

Difference 11.4.3 Tuple and List 

11.4.4 knowledge points 

Learn Python 11.4.5 System 

##  11.4.1 Immutable Data Types 

Immutable data types refer to data types that cannot be modified, i.e. read-only. The immutable data types learned so far are string, tuple. 

![avatar]( 5edecbf62dc874a327bac9ea6108a816.png) 

When using the [] operator to modify strings and tuples, Python will throw an exception message with the wrong type, which we can verify in interactive mode: 

>  >>> content = "static data type"

> >> content[0]=S

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

NameError: name 'S' is not defined

> >> numbers = (1,2,3,4,5)

> >> numbers[0] = 6

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

TypeError: 'tuple' object does not support item assignment 

The Python interpreter throws an exception message for TypeError, which means type error. The reason why it is a type error is easy to understand, because the type string or tuple does not support modifying elements. 

##  11.4.2 Variable Data Types 

The opposite of immutable data types is mutable data types, in which elements in a collection can be modified. Lists, as well as composite data types such as dictionaries, collections, class types, etc. that will be introduced later, are mutable data types. We can also verify this in interactive mode: 

>  >>> numbers = [1,2,3,4,5]

> >> id(numbers)

2749153235976

> >> numbers[0]=6

> >> numbers

[6, 2, 3, 4, 5]

> >> id(numbers)

2749153235976 

From the output of the interactive mode, it can be analyzed that it can be modified by the [] operator list type. The modified list has the same id value as the modified list, indicating that it is the same list. 

>  Call the built-in id function to get the id value of the object. In CPython, the id value is the memory address. 

##  Difference 11.4.3 Tuple and List 

In scenarios where tuples are used, lists can be used instead, so why define the data type tuples? In the content of this section, the analysis is carried out through two aspects: 

Tuples are static, read-only data types 

The core difference between tuples and lists is that tuples are static and immutable, while lists are dynamic and mutable. When we define variables, we should use tuples if the data object has static, read-only properties, otherwise we should use lists. Take the example of a shopping list in life. In the shopping list, we can modify the list at any time, such as adding a certain item or removing a certain item from the shopping cart. The shopping list is modifiable, dynamic, and now simulated through Python code: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590576
 ```  
There are seven days in a week, from Monday to Sunday, and no other time units are included. At this time, it is very natural to use tuples to define all the times of the week: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590576
 ```  
Since lists are mutable data types, they can be modified at any time in the program. 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590576
 ```  
The time of the week includes the eighth day, which is obviously not in line with daily logic. Using tuples can avoid such problems. Once the tuple is modified, Python will throw an exception message with the wrong type. 

(2) Automatic unpacking of tuples 

In Section 11.1, it was mentioned that tuples can be unpacked. With this feature, it is possible to assign values to multiple variables very elegantly. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590576
 ```  
We will systematically learn functions in Python in later courses. Returning multiple values in a function essentially returns a tuple. Using the automatic unpacking of tuples, variables can be elegantly assigned after a function call. 

##  11.4.4 knowledge points 

>  (1) A static data type refers to a data type that cannot be modified, i.e. read-only. The static data types learned so far are string and tuple.

(2) The opposite of static data types is dynamic data types, which support the modification of elements in a collection. Lists, as well as other composite data types: dictionaries, collections, class types, etc., are all dynamic data types. 

##  Learn Python 11.4.5 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

