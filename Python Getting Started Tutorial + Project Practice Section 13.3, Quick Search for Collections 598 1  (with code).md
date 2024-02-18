directory 

13.3.1 key output order 

13.3.2 key data type 

Quick lookup of 13.3.3 collections 

13.3.4 knowledge points 

Learn Python 13.3.5 System 

##  13.3.1 key output order 

The underlying implementation of a collection type is based on a hash table, and the order in which keys are output depends on the order in which they are stored in the hash table. 

![avatar]( ee84716de2f888a82a8719b0322d07be.png) 

>  Students who are not familiar with the hash table structure can review the content in 12.4.4 section. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574543774
 ```  
From the output of the program, it can be seen that the output order of the keys in the collection is not necessarily the order in which they were defined or inserted. Students can compare the output order of the keys in the dictionary. After Python 3.6, the keys in the dictionary are output in the order in which they were inserted: 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574543774
 ```  
From the output of the program, it can be analyzed that the output order of the keys in the dictionary is consistent with the order of the keys. 

##  13.3.2 key data type 

The data type of the keys in the collection is the same as the data type of the keys in the dictionary, and must be a static, hashable data type. 

>  The static data types I have learned so far are: simple data types, strings, and tuples. 

Why do keys have to be static data types? 

The collection type in Python is also based on a hash table structure. If the key name is static and immutable, then it is guaranteed that the same hash value will be obtained when computed through the hash function. If the key name is a mutable data type, it means that its value changes during the lifetime of the data type, and there is no guarantee that the computed hash value is the same, so the key name must be a static data type to ensure the uniqueness of its hash value. 

##  Quick lookup of 13.3.3 collections 

The collection type is based on a hash table structure, so it can also perform fast lookups. But unlike the dictionary type, there are only keys in the collection, not key values. The collection type is suitable for such application scenarios: it is only used for fast lookups, and there is no need to care about the key value corresponding to the key. When we still need to get the key value, we should use the data structure of the dictionary. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574543774
 ```  
##  13.3.4 knowledge points 

>  (1) The underlying implementation of the collection type is based on a hash table, and the output order of the keys depends on the order in which the keys are stored in the hash table

(2) The data type of the key in the collection must be a static data type. The static data types learned so far are: simple data type, string, tuple.

(3) The collection type, like the dictionary type, is a data structure implemented based on a hash table. 

##  Learn Python 13.3.5 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

