directory 

14.5.1 understand function decorators 

14.5.2 understand closure functions 

14.5.3 extend functionality with closures 

14.5.4 more elegant approach: decorator syntactic sugar 

14.5.5 knowledge points 

Learn Python 14.5.6 System 

##  14.5.1 understand function decorators 

Before getting to the main topic, let's take a look at the explanation of the words "decoration". The following content is quoted from Baidu Encyclopedia: 

>  Decoration, "Ci Yuan" explained as "the person who decorates, the person who hides, the person who decorates, the thing is done and the literary style is also." Refers to adding patterns and colors to the surface of utensils to achieve the purpose of beautification. 

"Decoration" itself contains the meaning of functional expansion, such as coloring objects, which is the expansion of color, and adding decorations to objects, which is the expansion of decorations. Our usual reading, fitness, and learning are also an expansion, through many ways to improve our inner and outer. 

![avatar]( 53ef863f730c0a841ea8813b3ab3432a.png) 

Using this analogy, it is easy to understand that decorators in programming languages are also used for functional extensions. In object oriented, decorators are a software design pattern that can extend existing objects functionally without changing their structure. 

>  In the course of Chapter 16, object oriented programming will be explained in detail. 

So, how can we use decorators to extend functionality? We need to learn about closure functions in Python first. 

##  14.5.2 understand closure functions 

A closure function, simply understood, is an inner function defined in a function that can access parameters and variables in the scope of the outer function. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
Code explanation: 

>  In the above code, a login function is defined, and a check function is defined inside the login function to check the user's login status. The login function is an external function of the check function, and inside the check function, the _USER_INFO variable in the login function is accessed. Functions like check are closures. 

##  14.5.3 extend functionality with closures 

Suppose we define a welcome page in web development, and you don't need to log in to enter the welcome page at first. Define a welcome function to simulate the output of the welcome page: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
As the project continues to iterate, the user is now required to log in before the welcome page pops up. How to extend the welcome function at this time? There are two expansion schemes: 

>  (1) directly modify the welcome function and check the user's login status within the welcome function

(2) Make the closure function share the same parameters as the welcome function, so that the user's login status can be checked in the closure function, and then the welcome function can be executed if the user is logged in. 

Adopting the first scheme will change the code logic of the welcome function. Adopting the second scheme is to transfer the extension logic of the code to the closure function. Now, the reader is invited to review the definition of the decorator pattern: to extend the functionality of an existing object without changing its structure. The second scheme adopted is the so-called decorator pattern. In Python's decorator pattern, its core is to use the closure function to extend the functionality of the decorated object. 

Now, through the second scheme, to check the user's login status, functions in Python can accept any type of parameter, and we can directly pass the welcome function as a parameter to the login function. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
##  14.5.4 more elegant approach: decorator syntactic sugar 

In 14.5.3 section, we extend the functionality of other functions through closure functions, but it is not intuitive and natural to use: 

>  (1) You need to pass the decorated function as an argument to the decorator

(2) The returned closure function needs to be executed again 

Python provides syntactic sugar, adding a line of @decortator modifier in front of the function header to decorate the current function, decortator represents the specific decorator name. In the above code, the login function is a decorator, and now use the @symbol to decorate the welcome function. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
After decorating the welcome function with @login, Python will automatically pass the wecome function as an argument to the login function and execute the returned closure function, which is the core logic of the Python decorator. The closure function parameters in the decorator must be the same as the parameters of the decorated object. When you are not sure about the parameters of the decorated object, you can use variable parameters: * args, ** kwargs. Decorator structures with variable parameters: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
When using decorator syntax sugar, decorators can also carry parameters, usually by nesting another layer of closure functions, defining the decorator's parameters in the outermost function of the decorator, and passing the decorated object in the second layer: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
Now continue to extend the welcome function to jump to the login page when the user is not logged in. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574526079
 ```  
In Python, decorators defined using function objects are called function decorators. Decorators defined using class types are called class decorators. This article focuses on function decorators, and the same principle applies to class decorators. 

>  In later lessons, the French Fries teacher will explain class decorators in Python in detail. 

The core of decorator is to extend the functions of existing objects without changing their structure. In actual development, we can extend the functions of cache, log output and so on for executable objects through decorator. 

##  14.5.5 knowledge points 

>  (1) Decorators are also used for functional extensions. In Object Oriented, a decorator is a software design pattern that extends an existing object functionally without changing its structure.

(2) A closure function, simply understood, is an inner function defined in a function that can access parameters and variables in the scope of the outer function. 

##  Learn Python 14.5.6 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

