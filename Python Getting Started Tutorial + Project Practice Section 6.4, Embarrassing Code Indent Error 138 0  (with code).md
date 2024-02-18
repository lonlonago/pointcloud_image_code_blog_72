directory 

 6.4.1 IndentationError 

6.4.2 What is code indentation 

6.4.3 code indentation rules 

6.4.4 meaning of code indentation 

Learn Python 6.4.5 System 

##   6.4.1 IndentationError 

When beginners learn Python, an IndentationError will be raised if they are not careful. For example, the following code: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
Now ask students to write the above example code into a Python script file, and then run the script on the command line or in the IDE. 

>  Students can review the content in Chapter 2 to learn how to run Python programs in the IDE. Review the content in Section 5.1 to learn how to execute Python programs on the command line. 

After running the script, the following error message appears on the command line or in the output window of the IDE: 

 File "demo.py", line 9

    Print ("Happy")

    ^

IndentationError: unexpected indent 

From the error message, an IndentationError appears on line 9 of the file. Open the source code file with PyCharm, and the IDE will mark a red wavy line at the beginning of the code that raises the exception: 

![avatar]( 77a4d97a199d38c9aab0e0897ae981b3.png) 

IndentationError is called a code indentation error in Python. If you write a program without following Python's code indentation rules, an IndentationError will be thrown during the execution of the program. 

>  IndentationError is a built-in exception type in Python that represents indentation errors. When students are beginners to Python, they will throw various exceptions without paying attention, such as common syntax errors, indentation errors, coding errors, etc. 

Exception is a built-in error handling mechanism in Python. When Python interprets and executes a program script, it will throw an exception once an error occurs. When an exception occurs, students should be good at analyzing the error message and find the key to solving the problem from the error message. 

##  6.4.2 What is code indentation 

Code indentation in programming languages refers to adjusting the distance between the code and the parent edge, which is measured by the number of spaces. For example, indenting four spaces means four spaces away from the parent edge. For example, the following code contains indentation: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
##  6.4.3 code indentation rules 

Python takes a mandatory indentation of code. Students must write code according to its indentation rules when writing Python programs, otherwise the program will report an error and throw an IndentationError error exception when running. The following is the summary of the French fries teacher, the code indentation rules in Python: 

>  (1) Global code does not require indentation, it must be top-level

(2) Statements at the same level must contain the same number of indented spaces

(3) child-level statements and parent-level statements must be indented

(4) Single-line comments can be indented at will, and multi-line comments maintain the same indentation as code at the same level 

Now let's explain the code indentation rules in Python through an example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
Students should note that although single-line comments can be indented at will, in actual development, they are usually indented at the same level as multi-line comments. 

>  The Tab key in the keyboard outputs whitespace characters. Its encoding in the computer system is different from the encoding of spaces. In some IDEs or editors, they automatically convert the output of the Tab key to 4 or 8 spaces. Students may need to make additional configuration when using the integrated development environment, otherwise it will bring problems on porting. The best practice is to use only the space bar to output spaces where code indentation is required, so there will be no errors. 

##  6.4.4 meaning of code indentation 

Code indentation allows you to distinguish the logical hierarchy of source code, such as the following code: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
From the writing form of the source code, it can be immediately seen that the child code block below the colon. Code indentation can standardize the writing format of the code, making the source code look neater and more beautiful as a whole. 

Code without indentation: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
Code to force indentation: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589966
 ```  
##  6.4.5 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

