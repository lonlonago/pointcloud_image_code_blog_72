directory 

8.1.1 understand data types 

8.1.2 Data Types in Python 

8.1.3 simple data types 

8.1.4 Special None Type 

Data Types of 8.1.5 Variables 

8.1.6 knowledge points 

Learn Python 8.1.7 System 

##  8.1.1 understand data types 

Data types are classified according to the properties and characteristics of the data itself. For example, odd and even numbers are a data type. In the data type of odd number, the elements in the data set are all odd, and the remainder after odd and 2 is 1. In the data type of even number, the elements in the data set are all even, and the remainder after even and 2 is 0. 

![avatar]( 96f981fb947fe227887ba8e34b4b0b2a.png) 

Data types are not limited to numbers. Anyone who can be converted into data form can define a type for it. Defining a type for data greatly facilitates human analysis and processing of data at the logical level. 

For a computer, there is no data type, it "sees" only binary, and the data type in a programming language is a logical concept defined to facilitate programmers' data processing.

In Chapter 11, we will introduce object-oriented programming, where we can build a data model through the semantics of objects, and we can customize data types. 

##  8.1.2 Data Types in Python 

Data types in Python are mainly divided into simple data types and composite data types. 

>  Simple data types are basic data types that can no longer be divided. Composite data types, on the other hand, can be composed of simple data types. 

The simple data types in Python are integers, floating-point types, and boolean types. Integers are what we often call integers. Floating-point types are those with decimal points. Boolean types are used to represent logically true and false. Compound data types in Python include string, list, tuple, dictionary, set, and class types, which will be explained separately in subsequent tutorials. In this section, we will thoroughly master the simple data types in Python. 

##  8.1.3 simple data types 

Data types have their own specific type names. In Python, you can output the type name of the data type through the built-in type type. basic usage of type: 

type(object) 

When you execute a type function, you can pass a value or variable name through the parameter object to output the corresponding type name. 

(1) Integer type 

Integer types are commonly referred to as integers, such as negative integers, positive integers, and 0. Now please enter the interactive mode of Python and output the type name of the data through the type type. 

> >> type(2020)

<class 'int'> 

In interactive mode, you can see the output of < class'int '>, with the type name of the data enclosed in single quotes. 

 Class has the meaning of class, category, and data types are defined in Python through the class keyword. 

We continue to verify the type names of other integers in interactive mode. 

> >> type(0)

<class 'int'>

> >> type(-1314)

<class 'int'> 

From the output of the interaction mode, we can find such a law. For integers, their type names are int. In the process of learning, it is a very effective learning method to continuously verify the input and output or logical concepts and find the laws of things in phenomena. 

(2) Floating point type 

Floating-point types are commonly referred to as decimals, with decimal points, such as 20.1314, 0.0. Likewise, the type name of a floating-point type can be output by type: 

> >> type(0.0)

<class 'float'>

> >> type(20.1314)

<class 'float'> 

A floating-point type in Python whose type name is float. When there is only a. sign at the end of the number, it is also a floating-point type. 

> >> type(0.)

<class 'float'> 

(3) Boolean type 

Boolean types are used to represent logically true or false. In Python, the True and False keywords are provided. The former is used to represent logically true values, and the latter is used to represent logically false values. Output the type name of the Boolean type in interactive mode: 

> >> type(True)<class 'bool'>>>> type(False)<class 'bool'> 

Boolean type in Python, whose type is called bool. Now write an example program using the simple data types described above. 

Code example - calculate the sum of all composite numbers between 1 and 10: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574597102
 ```  
The code in the above section implements the same function as the code examples in the 7.2.4 section. The main changes are as follows: 

>  (1) Change the outer loop to the for loop

(2) Define the variable is_composite_number as a Boolean type. In practical development, if you need to represent logical true or false, then it is more natural to use a Boolean type. 

0 values of integer and floating-point types are automatically converted to logical false values. In Python, True is used for true values, and False is used for false values. 

##  8.1.4 Special None Type 

There is a special None type in Python. None semantically represents the null data type. It is a singleton with a constant None value. None is a keyword in Python that indicates that the value is null. Now enter the interactive mode and see the corresponding type of None: 

> >> type(None)

<class 'NoneType'> 

From the output, the corresponding type of None is NoneType. In Python, the value of None is only equal to the value of None, and the Boolean value converted to None is False. 

##  Data Types of 8.1.5 Variables 

Variables are a container used to store data memory addresses. The type of a variable depends on the type of data the variable points to. We can also verify this in interactive mode: 

> >> data_type = 0

> >> type(data_type)

<class 'int'>

> >> data_type = 20.1314

> >> type(data_type)

<class 'float'>

> >> data_type = True

> >> type(data_type)

<class 'bool'> 

##  8.1.6 knowledge points 

>  (1) Data types are classified according to the nature and characteristics of the data itself

(2) The simple data types in Python are integer, floating-point, and boolean. The type of the integer is named int, the type of the floating-point type is named float, and the type of the boolean type is named bool. True in the boolean type is used to represent true values, and False is used to represent false values.

(3) Python also provides the None type, which semantically represents the null type.

(4) The data type of a variable refers to the type of value that the variable points to. 

##  8.1.7 the most powerful small class training 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

