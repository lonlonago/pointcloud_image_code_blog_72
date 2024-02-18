directory 

7.1.1 understand conditional control 

7.1.2 if,elif,else 

7.1.3 conditional expression 

7.1.4 conditional controls can be nested 

7.1.5 if statement ternary operation 

Learn Python 7.1.6 System 

##  7.1.1 understand conditional control 

In daily life, we often like to say if, "what if, then what will happen". "What if" expresses a hypothetical situation, that is, if the hypothesis is true, a certain operation will be performed, and if the hypothesis is not true, the same operation will be performed. 

For example, in the following "if" sentence: 

>  If it is sunny tomorrow, I will go to climb Lotus Mountain. Otherwise, I will go to the coffee shop downstairs and have a cup of coffee. 

The assumptions made in the above sentence are: 

>  It will be sunny tomorrow. 

The operation performed when the assumption is true: 

>  Climb Lotus Mountain 

The action performed when the assumption is not true: 

>  Drink coffee 

This kind of logical structure expressed in "if" sentences is a kind of conditional control. The core of conditional control is to first propose a hypothetical condition, if the condition is true, what kind of operation is performed, and if the condition is not true, continue to judge other conditions. In programming languages, conditional control is also carried out through "if", which corresponds to the keyword "if", and the Chinese definition of if is "if". 

##  7.1.2 if,elif,else 

In Python, if, elif, and else are used for conditional control. 

>  Students can find the definition and usage of the if, elif, and else keywords in the interactive mode. Take if as an example: help ("if"). 

Syntax structure of conditional control: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
If means if. Expression is a conditional expression in the conditional control structure. Usually, anything that can output a value can be used as a conditional expression. If the value of the conditional expression is true value, then the corresponding operation. elif is used to represent a branch condition, that is, if the condition in the if statement is not satisfied, continue to determine whether the condition in the elif statement is satisfied. Else represents an operation performed when the conditions in the if statement and the elif statement are not satisfied. 

>  The colon in the syntax structure indicates the beginning of a conditional block. In the syntax structure of conditional control, elif and else are not necessary. There can be multiple elif, but only one else at most. 

Illegal conditional control structure: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
In the above illegal conditional control structure, there are multiple else statements. The elif statement must follow the if statement, and the else statement must be the last statement in the control structure. 

Illegal conditional control structure: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
In the above illegal conditional control structure, the elif statement must follow the if statement, and the else statement must be the last statement in the control structure. When there are multiple if statements, Python treats each if statement as a separate conditional control structure: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
##  7.1.3 conditional expression 

If the value of the conditional expression is true, then the corresponding operation is performed. 

Code example (1): 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
In the above code example, a is_happy variable is defined, which points to a value of 0, and the logical value converted from 0 is false. So the code in the if statement will not be executed, but the code below the else statement will be executed, and the output is: 

i am so unhappy 

Code example (2): 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
In the above code example, an x variable is defined, which points to the value 1, and a y variable is defined, which points to the value -1. The value of x + y is 0, so the expression x + y > 0 is equivalent to 0 > 0. Obviously, the value of the expression is false, so we will continue to determine whether the condition in the elif statement is true. The conditional expression in elif is "x + y == 0", and the value of the expression is true, so the code in the elif statement will be executed: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
The output of the final program is: 

x+y == 0 

Code example (3): 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
In the above code example, an x variable is defined, which points to the value -1, and a y variable is defined, which points to the value -1. The value of x * y is 1, so the value of the expression x * y > 0 is true. The value of x + y is -2, so the value of the expression x + y > 0 is false. The conditional expression in the if statement is "x + y > 0 and x * y > 0", which is equivalent to "true and false". In the logical AND operation, as long as one of the logical values is false, then the output is false. Therefore, the next conditional branch will be judged: 

elif x+y > 0 

The value of the expression x + y = 0 is false, and Python will proceed to determine the next conditional branch: "elif x * y > 0". The value of the expression x * y > 0 is true, so the code below the colon is executed: 

Print ("Both x and y are negative") 

The output of the final program is: 

Both x and y are negative 

Students need to clarify the judgment logic in the code when analyzing the execution process of the above code. Why are both x and y negative? 

##  7.1.4 conditional controls can be nested 

Nesting means that conditional statements can be nested under conditional statements. Readers should pay attention to the code indentation when the if statement is nested. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
The program output is: 

i'm so happy to learn Python!

Both x and y are negative 

If the depth of the nesting should not be too deep, it is usually kept within three layers. Too many nesting layers will lead to poor readability of the code and difficult to maintain. 

##  7.1.5 if statement ternary operation 

Ternary operators are a fixed format in software programming. In Python, ternary operators are implemented through if statements. 

Syntax format of ternary operators: 

expression1 if condition_expression else expression2 

The execution logic of the ternary operator is: if the value of the conditional expression condition_expression in the if statement is true, return the value of the expression expression1, otherwise return the value of the expression expression2. 

Using ternary operators can simplify the use of if statements in specific scenarios. 

Code examples that do not use ternary operators: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
Code example using the ternary operator: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586447
 ```  
These two code examples achieve the same effect, but the code using the ternary operator looks more concise. In the case of more conditional branches, it is not suitable to use the ternary operator. Readers need to use it reasonably according to the actual situation. 

##  Learn Python 7.1.6 System 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

