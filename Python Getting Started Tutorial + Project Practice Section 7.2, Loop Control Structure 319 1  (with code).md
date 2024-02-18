directory 

7.2.1 understand circular control 

7.2.2 for loop structure 

7.2.3 while loop structure 

7.2.4 loop structure can be nested 

7.2.5 knowledge points 

Learn Python 7.2.6 System 

##  7.2.1 understand circular control 

To understand loop control, you must first understand what a loop is. The following is quoted from a Chinese dictionary: 

Cycle means to go back and forth, when something moves or changes over and over again, or does something repeatedly and continuously

![avatar]( fb4fea5bb903d9c813b2f4bceca284d1.png) 

Then, by analogy in a programming language, it is easy to understand loop control: controlling the repeated execution of a program through certain instructions. By controlling the repeated execution of program instructions, programmers can be freed from the tedious work of writing code. Students first consider the following question: 

Calculate the sum of all natural numbers between 1 and 10

At first glance, it seems like a very simple problem. To solve this problem, simply list all the natural numbers between 1 and 10, and then add them directly. 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
But if the problem is changed to "calculate the sum of all natural numbers between 1 and 100,000", how to write the program code? It is very inefficient to add numbers by hand. For such problems, the loop control in the programming language can provide the perfect solution. 

##  7.2.2 for loop structure 

In Python, the loop structure is defined by the for and while keywords, and the else statement in the loop structure is used to define the operation to be performed when the loop exits normally. 

>  Students can find the definition and usage of keywords such as for and while in the interactive mode, and develop a good habit of searching in the interactive mode. For example, find the definition and usage of the for keyword: help ("for"). 

(1) for loop basic grammar 

The grammatical structure of a for loop: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
target_list represents a list of target values, expression_list represents a list of expressions, and the else statement in the loop is used to define the operation performed when the loop exits normally. In the for loop structure, the values in the expression list are traversed one by one, and then the values are assigned to the parameter target_list. In Python, expression lists can be defined directly through English commas, such as: 

1,2,3,4,5 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

1

2

3

4

5 

Code Explanation: 

The for loop iterates through the values in the expression list one by one, and then assigns the traversed values to the variable number. The value in the expression list is (1, 2, 3, 4, 5), and there are 5 values in the set, so the for loop iterates over 5 times, each time assigning the traversed value to the variable number. For example, the first traversed value is 1, and then assigned to the variable number, the second traversed value is 2, and the same is assigned to the variable number, and so on. 

Comma-separated expressions are actually tuple types in Python, which will be explained in detail later when introducing data types. 

(2) The else statement in the for loop 

The else statement in the loop is not necessary. If you want to define the operation to be performed when the loop exits normally, you need to add an else statement to the for loop structure. The else in the for loop structure is usually used to define the closing operation after the loop exits normally. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

1

2

3

4

5

The for loop exits normally 

(3) Execute the break exit loop 

The so-called abnormal exit of the loop refers to the execution of the break command in the loop. When Python is interpreting the execution of the script, if it finds that the current instruction is break, it will immediately exit the current loop. 

>  The break command can only be used in a loop structure. If used elsewhere, Python will throw an exception message with a syntax error. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

1

2

3

4 

(3) range type 

Python provides a range type that can be used to generate integer sequences. Basic usage of the range type: 

range(start, stop[, step]) 

The parameters start and stop are used to construct a left-closed and right-open interval [start, stop) of the integer sequence. Assuming the value of start is 0 and the value of stop is 5, then the left-closed and right-open interval is [0, 5). The integer sequence corresponding to the range (0, 5) is: 

0,1,2,3,4 

Step is an optional parameter. The so-called optional parameter can be filled in or not. The step parameter is used to represent the step size between adjacent numbers. Continuing to take the left-closed and right-open interval [0, 5) as an example, assuming the step size is 2, the integer sequence corresponding to range (0, 5, 2) is: 

0,2,4

The starting number is 0, so the next number is 0 + 2, which is 2.

The next number in #2 is 2 + 2, which is 4. Students can do the same. 

When passing only one parameter to the range type, a forward interval is constructed from 0 to that parameter. For example, when passing the parameter value 5, the forward interval is constructed as [0, 5). When the passed parameter value is less than or equal to 0, no integer is generated. When the step size passed to the range type is negative, a descending sorted sequence of integers can be generated. At this time, the value of start must be greater than the value of stop. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

5

4

3

2

1 

Using the integer sequence generated by the range type, and then through the loop structure, the sum of all natural numbers between 1 and 10000 can be calculated. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

50005000 

50005000 is the sum of all natural numbers between 1 and 10000. 

##  7.2.3 while loop structure 

(1) While loop basic syntax 

The grammatical structure of the while loop: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
Expression represents an expression. When the value of the expression is true value, the code below the while will be executed in a loop. The else in the while is the same as the else in the for loop, which is used to define the operation to be performed when the loop exits normally. You can also execute break in the while loop to exit the loop. 

View the definition and usage of the while keyword in interactive mode: help ("while") 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The expression in while is 0, and the value of 0 is false, so the print function in the while loop will not be executed. 

>  In everything I've learned so far, both 0 values and empty strings are false values. An empty string is a quote without any characters inside. For example, "" is an empty string. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
The program output is: 

x+y=4

x+y=2

x+y=0 

Code explanation: 

>  The initial values of x and y are both 3, and the value of x + y is 6, so the value of x + y > 0 is true. In the while loop, the values of x and y are continuously reduced by -1. When the values of x and y are both 0, x + y = 0, then the value of the expression x + y > 0 is false, so the code in the loop body will not be run. 

![avatar]( 18519c1f9c5ce5f2d60d7655c52a0051.png) 

##  7.2.4 loop structure can be nested 

Loop structure, like conditional control structure, can also be nested. Similarly, pay attention to code indentation when nesting, and the depth of nesting should not be too deep, otherwise it will lead to poor readability of the code and difficult to maintain. 

Code example - calculate the sum of all composite numbers between 1 and 10: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574594121
 ```  
In the above code example, the for loop is nested in the while loop, and the while loop can also be nested in the while loop, and the for loop can be nested in the for loop. Students can change all the code examples above to the for loop structure to compare the difference between the use of the while loop and the for loop. 

##  7.2.5 knowledge points 

>  (1) Cyclic control refers to the repeated execution of a program through instructions

(2) Python uses for, while to implement loop control

(3) When break is used in a loop, it indicates an abnormal exit

(4) The else statement in the loop structure is used to define the operation after the loop exits normally

Python's built-in range type can be used to generate a sequence of integers 

##  Learn Python 7.2.6 System 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

