directory 

Formatting 12.3.1 string 

12.3.2 formatting using a dictionary 

Advantages and disadvantages of 12.3.3 formatting operation method 

12.3.4 knowledge points 

Learn Python 12.3.5 System 

##  Formatting 12.3.1 string 

In Section 9.4, we introduced string formatting. Let's first review the definition of string formatting and the main formatting methods: 

>  String formatting refers to the output of strings in a specific format. There are two main ways to format strings: one is through the operator%, and the other is through the format method of the string type. 

![avatar]( eb74598d5090d22725082489f96dc229.png) 

In this section, we focus on formatting strings with dictionary types. 

##  12.3.2 formatting using a dictionary 

When using a dictionary for formatting operations, it is mainly formatted by means of keyword placeholders. Here, the keyword placeholder corresponds to the key name in the dictionary, and the key name appears in the string to be formatted. When formatting the string, the Python interpreter automatically replaces the keyword placeholder in the string with the corresponding key value. 

(1) Format with% and dictionary 

Formatting syntax: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
The key represents the key name in the dictionary, and the s indicates that the keyword placeholder is formatted as a string type. You can also replace the s with other formatting types, such as d, which is formatted as an integer, and f, which is formatted as a floating-point type. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
The keyword placeholder in the string must be able to match the corresponding key name in the dictionary, otherwise Python will throw an error exception that the key name does not exist, and students can verify it in interactive mode: 

>  "The author of this book is% (author) s " % ({})

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

KeyError: 'author' 

(2) Format with a dictionary 

1. Pass the dictionary object as a keyword parameter in the format method 

Formatting syntax: 

>  "{param[key]}".format(param=dict) 

The placeholders to be formatted in the string are in the same form as the dictionary and are enclosed in {}. The corresponding key value is output in the form of key name access in {}. In the format method, the dictionary object is passed in the form of keyword parameters. When calling a function in Python, the parameter passing form of name = value is the passing syntax of keyword parameters. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
Similarly, the keyword placeholder in the string must match the corresponding key name in the dictionary, otherwise Python will throw an error exception that the key name does not exist. Students can continue to verify in interactive mode. 

2. Use the ** symbol to unpack the dictionary 

Formatting syntax: 

>  "{key}".format(**dict) 

The key in {} represents the key name in the dictionary. When unpacking the dict with ** in the format method, it will be expanded in format to the form of the keyword argument passed with name = value. Name is the key name in the dictionary, and value is the key value corresponding to the key name. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
You can also format a string directly in the form of keyword arguments, achieving the same effect: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
##  Advantages and disadvantages of 12.3.3 formatting operation method 

Before explaining the advantages and disadvantages of formatting operations, let's take a few simple examples: formatting through format symbols and dictionary types, respectively. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
When formatting with a format symbol, Python performs type checking, and the data type must be consistent with the type represented by the format symbol or can be implicitly converted to the corresponding data type, otherwise an exception message of type error will be thrown. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
When using a dictionary type for formatting operations, there is no type checking, only text substitution, which is more readable than formatting operations. Strings using formatting symbols: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
A string formatted with a dictionary type: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522779
 ```  
##  12.3.4 knowledge points 

>  (1) String formatting refers to the output of strings in a specific format. There are two main ways to format strings: one is through the operator%, and the other is through the format method of the string type.

(2) When using a dictionary for formatting operations, it is mainly formatted by means of keyword placeholders. The keyword placeholders here correspond to the key names in the dictionary

(3) The keyword placeholder in the string must be able to match the corresponding key name in the dictionary, otherwise Python will throw an error exception that the key name does not exist 

##  Learn Python 12.3.5 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

