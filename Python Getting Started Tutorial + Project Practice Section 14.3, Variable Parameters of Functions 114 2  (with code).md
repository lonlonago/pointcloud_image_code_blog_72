directory 

14.3.1 understand variable parameters 

14.3.2 operators * and ** 

14.3.3 unpacking arguments 

14.3.4 knowledge points 

Learn Python 14.3.5 System 

##  14.3.1 understand variable parameters 

Variable parameters of a function can be understood from its literal meaning. "Variable" means that the number of parameters is variable and uncertain. When defining a function in Python, add a "*" or "**" modifier to the parameter, then the parameter is a deformable parameter. 

![avatar]( aa24ffc6cb8403250fb2b57e024c7730.png) 

##  14.3.2 operators * and ** 

(1) Use * to collect arguments as tuples 

When defining a function in Python, a "*" operator is preceded by a parameter, so when executing a function call, the Python interpreter will collect all the arguments starting at the position of the parameter into a tuple. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
>  The order of collection of deformable parameters is to start from the position of the deformable parameters and collect them from left to right 

Since deformable parameters are collected from left to right, we usually place deformable parameters to the right of ordinary parameters when defining functions. If deformable parameters are placed to the left of ordinary parameters, then in order for ordinary parameters to work, function calls must be made in the form of keyword parameters. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
(2) Use ** to collect arguments into a dictionary 

When defining a function, use the ** operator to decorate the parameter, and pass the parameter as a keyword parameter when calling the function, then Python will collect the argument at the beginning of the parameter position as a dictionary type. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
(3) Mixing "*" with "**" 

Use a mix of * and ** operators to decorate parameters. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
(4) *args 追**kwargs 

* Args and ** kwargs are common ways to write deformable parameter names. The former is used to package arguments into a tuple type, and the latter is used to package arguments into a dictionary type. Students can follow this general way of writing when actually defining functions, or they can define variable parameter names by themselves. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
##  14.3.3 unpacking arguments 

When defining a function, using * or ** collects arguments into a tuple or dictionary. When using * or ** to decorate a function, it unpacks arguments. The so-called unpacking is to take the elements in the data set and assign them to the corresponding parameters. To understand this usage, let's take a look at a code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
In the above code, the accumulate function has two parameters, number1 and number2. There are two elements in the actual parameter numbers. After unpacking numbers, the parameter corresponding to element value 1 is number1, and the parameter corresponding to element value 2 is number2. Then, calling accumulate (* numbers) is equivalent to calling accumulate (1,2). 

(1) Use * to unpack the iterable object 

Iterable objects learned so far are: string type, list, tuple, dictionary, collection. When unpacking dictionaries, collections, etc., the elements unpacked are the corresponding key names. In actual development, the ** operator is usually used to unpack dictionaries. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
(2) Use ** to unpack the dictionary 

When unpacking the dictionary, the key name in the dictionary corresponds to the parameter name in the function one-to-one, and the argument is the key value corresponding to the key name. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
The key names in the dictionary must correspond one-to-one with the parameter names in the function, otherwise Python will throw an exception message with the wrong type. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591602
 ```  
When the above code is executed, the program throws an exception message with a wrong type because the dictionary key name median cannot find the corresponding parameter name in the accumulate function. 

##  14.3.4 knowledge points 

>  (1) When defining a function, use the * and ** operators to define variable parameters, and when calling a function, use the * and ** operators to unpack the parameters.

When using the * operator to define a variable parameter, Python collects arguments starting at the parameter position into a tuple.

(3) When using the ** operator to define a variable parameter, Python collects the arguments starting at the parameter position into a dictionary. 

##  Learn Python 14.3.5 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

