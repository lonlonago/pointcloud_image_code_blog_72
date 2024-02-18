directory 

8.3.1 understand data type conversion 

8.3.2 explicit type conversion 

8.3.3 implicit type conversion 

Conversions 8.3.4 Other Types to Boolean Types 

8.3.5 Knowledge points in this section 

Learn Python 8.3.6 System 

##  8.3.1 understand data type conversion 

Data type conversion, as the name implies, is the conversion from one data type to another. The term "rounding" is often used to imply type conversion, that is, converting a floating-point decimal to an integer. 

![avatar]( f410f1a5e3c3bd78aece20d1d58c7149.png) 

In our daily lives, we often switch between various roles. In the enterprise, we are the boss or employee, at home, we are the husband or wife. We are polite to strangers, and we expose all kinds of bad temper to familiar people. This is also a type conversion. Type conversion can be said to be present all the time and everywhere. 

You need to have good expectations for life, although it is full of twists and turns and tribulations, don't forget who you are, but become what you want to be 

##  8.3.2 explicit type conversion 

From a literal perspective, explicit type conversion is the explicit conversion from one data type to another. In Python, explicit type conversion is achieved through the syntax of type name + (). 

Code example - round decimals: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515037
 ```  
Code explanation: 

(1) A floating-point variable of type money is defined in the code instance, and then the floating-point type is explicitly converted to an integer in the form of int (money).

(1) When converting an integer to a floating-point type, there is an extra decimal point after the number. For example, if you convert 201314 to a floating-point type, the converted value is 201314.0. 

Code example - Conversion between string type and numeric type: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515037
 ```  
Code explanation: 

>  (1) When converting a string type to a numeric type, explicitly convert the string type to a numeric type directly through int () or float ()

(2) For integers, the base of the conversion can be specified by the argument base in the explicit conversion of int (). When the number in the string represents decimal, the argument passed is 10.

  When the number in the string represents binary, the argument passed is 2. When the number in the string represents hexadecimal, the argument passed is 16.

(3) Convert numeric type to string type via str () 

When converting a string type to a numeric type, the content of the string must be a continuous legal number (decimal number, binary number, hexadecimal number, etc.), with space characters and plus or minus signs, and no other non-numeric characters. 

Code instance - string illegal conversion: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515037
 ```  
Code explanation: 

(1) string "20.1314 748" is not a consecutive number

(2) string "20.1314\ n" contains illegal characters 

##  8.3.3 implicit type conversion 

When using numeric types for numeric operations, data types with a small range are automatically converted to data types with a large range. Numeric types in Python: 

Boolean type, integer type, floating point type

Sort them by the size of the indicated range as follows: 

Boolean < integer < floating-point type

Code example - Implicit conversion of numeric types: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515037
 ```  
Code explanation: 

(1) Data types with a small range are automatically converted to data types with a large range

(2) In the expression 1 + 1.0 + True, 1 + 1.0 is computed first according to left associativity, 1 is an integer, 1.0 is a floating-point type,

Integer 1 is automatically converted to floating-point type 1.0, and the result of 1 + 1.0 is 2.0. Similarly, 2.0 + True is equivalent to 2.0 + 1.0, with a value of 3.0.

![avatar]( 8293169868493c64d70f04006d52b756.png) 

##  Conversions 8.3.4 Other Types to Boolean Types 

Each data type has its corresponding false value, and all converted boolean types that represent false values are False. False values in integers are 0, false values in floating-point types are 0.0, false values in string are empty string, None type represents empty type, and Boolean types after null type conversion are False. 

In conditional control structures and loop control structures, the value of an expression is converted to a logical value, and if it is a true value, the corresponding code is executed.

##  8.3.5 Knowledge points in this section 

(1) Data type conversion refers to the conversion of one data type into another

(2) Data type conversion in Python includes explicit type conversion and implicit type conversion 

(3) 0 values of integer and floating-point types, empty strings, None types, etc. are converted to False Boolean types.

##  Learn Python 8.3.6 System 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

