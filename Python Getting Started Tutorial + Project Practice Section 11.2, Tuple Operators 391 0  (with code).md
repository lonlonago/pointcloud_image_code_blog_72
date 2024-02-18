directory 

Common Operators 11.2.1 Tuples 

11.2.2 [] operator: index access tuple 

11.2.3 [:] operator: slice of tuple 

11.2.4 + operator: tuple addition 

11.2.5 * operator: multiplication of tuples 

Relational Operations 11.2.6 Tuples 

11.2.7 in operator: find element 

11.2.8 knowledge points 

Learn Python 11.2.9 System 

##  Common Operators 11.2.1 Tuples 

A tuple type is an abstract data type that defines how to operate on a data type. In this section, we focus on manipulating tuples through operators. 

![avatar]( 8f7c318a31a2c57c94790e31edfe50f1.png) 

The commonly used operators for tuple types are shown in the following table: 

![avatar]( 457c64d99904af3193690b9bcfad55b1.png) 

##  11.2.2 [] operator: index access tuple 

In Section 9.2, we introduced how to access the characters in a string by indexing. The tuple type is also a linear sequence structure, and like a string, the elements in the tuple can be accessed by indexing. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
Tuple and string are static data types, which can only be read by indexing characters and cannot be modified. The list type can be modified by indexing elements. 

>  Indexes in Python are divided into positive and negative indices. Positive indices are numbered from 0 and represent the first element in the data set. Negative indices are numbered from -1 and represent the first to last element in the data set. Positive and negative index values must be within a valid range or an out-of-bounds access error message will be thrown. Students who are not familiar with this can review the content in Section 9.2. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  11.2.3 [:] operator: slice of tuple 

The trimming operation syntax is the same as the slicing operation of string. For students who are not very familiar with this, please review the content in Section 9.2. After slicing a tuple, a new tuple is returned. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  11.2.4 + operator: tuple addition 

Tuple addition is the process of combining elements from two tuples into a new tuple. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  11.2.5 * operator: multiplication of tuples 

The "*" operator is used to repeat the output of the tuple and return a new list. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
The parameter number must be an integer number. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  Relational Operations 11.2.6 Tuples 

Use relational operators to perform relational operations on tuples and return a result of type Boolean. The relational operations of tuples are the same as the relational operations of lists. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
The relationship operation of tuples is compared in order. The order comparison here starts from the first element of the tuple and is compared element by element. Only if the element values are the same and the order is the same, the two tuples are equal. Otherwise, the size relationship of the tuples is determined by the size relationship of the elements. 

>  For example, in the code above, although the list right has only one element, the first element in right is greater than the first element in the list left. At this time, Python will directly determine that the tuple right is greater than the tuple left, even if the elements behind the tuple left are larger than the elements in the tuple right. 

Now use the loop structure to determine whether two tuples are equal: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  11.2.7 in operator: find element 

Use the "in" operator to determine whether the element exists in the tuple, and return a boolean type True if present, or False otherwise. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
When indicating whether it does not exist, the logical NOT operator is required. 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574540265
 ```  
##  11.2.8 knowledge points 

>  (1) A tuple type is a linear sequence structure in which elements in a tuple can be accessed by indexing.

(2) Tuple and string are static data types that can only be read by indexing characters and cannot be modified. List types can be modified by indexing elements.

(3) The relationship operation of tuples is compared in order. The order comparison here starts from the first element of the tuple and is compared element by element. Only if the element values are the same and the order is the same, the two tuples are equal. Otherwise, the size relationship of the tuple is determined by the size relationship of the elements. 

##  Learn Python 11.2.9 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

