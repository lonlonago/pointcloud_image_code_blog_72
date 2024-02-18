directory 

7.3.1 understand steering control 

7.3.2 break - exit the entire loop 

7.3.3 continue- exit this cycle 

7.3.4 return-exit function execution 

7.3.5 knowledge points 

Learn Python 7.3.6 System 

##  7.3.1 understand steering control 

So far, we have learned about conditional control and loop control. In this section, we will learn about the last control structure in Python: turn control. Before learning anything new, let's review the definition of conditional control and loop control: 

Conditional control refers to the conditional execution of instructions in a program according to the value of the expression. Loop control refers to making program instructions execute continuously and repeatedly 

Understanding steering control can be understood from its literal meaning. Steering means reversing the direction, and controlling the execution of the code through steering control during the execution of the program. In the content of Section 7.2, steering control has actually been touched. Exiting the loop through break is a kind of steering control. In Python, steering control is realized through break, continue, and return, which will be explained in the following sections. 

![avatar]( 7b98ac9a914b1e9b86d815c3dec72bbc.png) 

##  7.3.2 break - exit the entire loop 

Break means break and break. Breaking the cycle means ending the cycle. In layman's terms, break is the terminator of the cycle, similar to the T-800 robot. 

Code example - Terminate the loop if it is greater than 2020: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457682
 ```  
Execute break to exit the loop, but only to exit the loop structure where break is located, without affecting the outer loop. 

Code explanation: 

(1) Use conditional controls in loops to determine the value sum_of_numbers variable points to

(2) If the value is greater than 2020, execute the break exit loop 

Code example - calculate the sum of all prime numbers 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457682
 ```  
Code explanation: 

(1) In the inner for loop, exit the current loop when number is divisible by other natural numbers.

(2) If the inner loop system exits normally, indicating that it cannot be divided by other natural numbers, then it is a prime number.

(3) Exiting the inner for loop will not affect the outer for loop. 

##  7.3.3 continue- exit this cycle 

Compared with break, continue only exits this loop. Assuming that it needs to be executed a total of 5 times in the loop, using break in the first loop will not execute the remaining 4 loops. Using continue in the first loop will end the current loop, and the remaining 4 loops will still execute. 

Code example - calculate the sum of all odd numbers: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457682
 ```  
Code explanation: 

(1) % is a remainder calculator in Python. If the remainder after the number is 2 is 0, it means it is an even number.

If it is even, the loop ends.

(2) If it is not even, then the code in the loop body continues to be executed to calculate the sum of all odd numbers. 

Code example - output an inverted triangle: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457682
 ```  
The program output is: 

* * *

 * *

  * 

Code explanation: 

>  (1) According to the characteristics of the graphics themselves, find patterns

(2) Obviously, there are three rows and five columns in the inverted triangle. Use the * symbol and the space symbol to jointly output the triangle

(3) When the number of the column is equal to the number of the row in this cycle, the * symbol is printed, which can be found from the characteristics of the graph itself.

(4) Furthermore, the number of * in each layer of the inverted triangle is decreasing and centered, and the effective range of the printed * is within the range of the number of columns minus the number of the current row. In Python, both break and continue can only be used for loop structures. Using break in a loop means that it exits abnormally and does not execute the code in the else. 

##  7.3.4 return-exit function execution 

In programming languages, return is used to exit the execution of a function, usually returning a value to the caller of the function. About functions, we will explain in detail in Chapter 14. 

 For the definition and usage of keywords such as break, continue, return, etc., students can also look up in the interactive mode and will not go into details.

##  7.3.5 knowledge points 

(1) Steering control is generally used in loop structures and functions to control the execution of loops and functions. 

(2) Python implements steering control through break, continue, and return. 

(3) break is to terminate the entire cycle, continue is to terminate this cycle 

(4) return is used to exit the execution of a function, usually returning a value to the caller.

##  Learn Python 7.3.6 System 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

