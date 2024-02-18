directory 

The concept of 6.1.1 variables 

Naming 6.1.2 variables 

Definition of 6.1.3 variables 

6.1.4 variable stores the address 

6.1.5 system to learn Python 

##  The concept of 6.1.1 variables 

After entering the fantasy forest of the programming world, the first obstacle that beginners will encounter is variables. Defining variables in Python is simple. A variable name, an equal sign, and a value can define a variable: 

Variable name = value 

But understanding the variables clearly requires some effort. 

So, what exactly are variables? 

Beginners can understand a variable as a container, such as the bottles and jars seen in ordinary life. The main purpose of these bottles and jars is to hold items. Since a variable is a container, it also has the characteristics of a container. In computer programs, variables are used to store data. Secondly, variables are constantly changing, but what changes is the data inside the container. For example, bottles and jars used to hold items, bottles and jars do not change, only the items in the bottle change. In a program, assigning variables to other variables is like transferring items from bottles to other bottles. 

![avatar]( e8aa9d494760d8ad3584b64d0bb69cb0.png) 

>  All the items in the bottle are dumped into other bottles, and the original bottle becomes an empty bottle. But in a computer program, just copying the value pointed to by the variable does not empty the value pointed to by the variable. 

##  Naming 6.1.2 variables 

(1) Naming rules 

People have names, and so do variables. Variables cannot be referenced in a program if they do not have names. For example, two unnamed variables are defined at the same time. How to refer to anonymous variables in code is a problem. People's names have their customary naming rules, usually named by surnames and first names. Variables in programming languages also have their own set of naming rules. Naming rules for variables in Python language: 

>  Variable names are usually 26 English letters (both upper and lower case), numbers and underscores _ combined, the first character of the variable name cannot be a number, variable names cannot use system predefined keywords 

>  Keywords in Python are reserved for Python use, so they can no longer be named using keywords. We will explain more later when we introduce the interactive mode. Execute help ("keywords") in the interactive mode to view all the keywords predefined by the system. In Python 3, you can use UTF-8 characters such as Chinese characters to name variables. 

Variable names must comply with the naming conventions in the programming language, otherwise they cannot run. A legal variable name does not mean a good variable name. A good variable name, usually named with English words, should not be too long, must have a certain meaning, and be readable. Not paying attention to the naming of variables, or even naming them at will, is a common problem for beginners. 

(2) Naming example 

Legal variable names: 

name, title, content 

Illegal variable name: 

1name,?title,content* 

In these three illegal variable names, the first variable name has a number at the beginning, the second variable name has an illegal character at the beginning, and the third variable name contains illegal characters. In addition, there is an important detail here, variable names are case-sensitive in Python, which means that Name and name represent different variables. 

(3) Naming style 

In postmodernism, which pursues diversity, "individual freedom," "self-contained system," and "critical right" have become a series of unique labels for followers. But in team development, the pursuit of diversity often leads to confusion. Using a unified naming style can improve the overall readability of the project code. The stronger the readability, the easier the project is to maintain. Three commonly used variable naming styles: 

Hump nomenclature, mixed nomenclature, underscore nomenclature 

In hump nomenclature, the first letter of a word is capitalized. 

Example of big hump nomenclature: 

PriceOfLove 

In the small hump nomenclature, the first word of a variable is all lowercase, and the first letter of all other words is uppercase. 

Examples of small hump nomenclature: 

priceOfLove 

The so-called underscore nomenclature is the underscore that connects words, and words are generally lowercase. 

Example of underscore nomenclature: 

price_of_love 

In Python, variable names are usually in lowercase, and the big hump naming convention is used to name class types. For more naming conventions, interested readers can refer to the famous PEP8 specification. 

##  Definition of 6.1.3 variables 

To use a variable in a program, you need to define the variable first, otherwise an error exception of "variable undefined" will be thrown during the execution of the program. Defining variables in Python is simple, use the = sign to define variables, for example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522122
 ```  
In the variable definition above, the variable name is total and the value is 66. When defining a variable, you can use a defined variable to assign values to other variables, such as: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522122
 ```  
In the variable definition above, Python will first take the value stored by the variable total, and then assign the value to the amount. The "value" here is the memory address in CPython. CPython is a Python interpreter. The Python we use, unless otherwise specified, usually refers to CPython. 

##  6.1.4 variable stores the address 

(1) Understanding the memory address 

The so-called address of memory is essentially a number. In a computer, memory can be regarded as a large array of bytes, which are numbered in sequence starting from 0. The following diagram shows the logical structure of memory in a computer: 

![avatar]( 2b3c9f843825b3d32fe31d2dd7e7c888.jpeg) 

The number in the figure is the memory address. Each cell represents a block of memory with a size of one byte. Assuming that the memory number where the value 66 is located is 2, then this 2 is the memory address of 66. 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522122
 ```  
The variable total essentially holds the memory address of the value 66:2. When assigning the variable total to the variable amount, Python mainly does the following two steps: 

One: remove the memory address of 66 from the variable total 2

Two: Assign memory address 2 of 66 to the variable amount 

The final variables total and amount both hold the same memory address, that is, they refer to the same piece of memory data. 

![avatar]( c47159ea3228ec6dacea836fca03de24.png) 

(2) Check the memory address 

In Python, you can output the memory address of a variable or value through the built-in function id. Just pass the variable or value as an argument to the id function. For example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574522122
 ```  
Interactive mode in Python is introduced in Section 6.5, which shows how to view the memory address of a variable or value through the id function. 

##  6.1.5 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

