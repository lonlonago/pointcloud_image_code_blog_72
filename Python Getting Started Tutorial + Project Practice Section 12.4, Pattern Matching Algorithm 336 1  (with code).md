directory 

12.4.1 What is pattern matching? 

12.4.2 naive pattern matching algorithm 

Learn Python 12.4.3 System 

##  12.4.1 What is pattern matching? 

Pattern matching is a basic operation of strings in a data structure: given a substring, it is required to find all substrings that are the same as the substring in the main string, which is pattern matching. For a simple example, the main string is "Chinese people do not bully Chinese people", and the substring is "China". The substring here is the pattern to be matched, and finding all the patterns "China" in the main string "Chinese people do not bully Chinese people" is a pattern matching. 

##  12.4.2 naive pattern matching algorithm 

This section aims to implement a very simple naive pattern matching algorithm. Let's first grasp the basic ideas of the naive pattern matching algorithm: 

>  From the first character of the main string, it is compared with the first character of the pattern string. If it is equal, the subsequent comparison of the characters is continued. Otherwise, it is re-compared with the first character of the pattern string from the second character of the main string. This process is repeated until each character in the pattern string is equal to a consecutive character sequence in the main string. At this time, it is called a match success, otherwise the match fails. 

According to the above ideas, we use the Python language to implement the naive pattern matching algorithm of string: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574532492
 ```  
##  Learn Python 12.4.3 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

