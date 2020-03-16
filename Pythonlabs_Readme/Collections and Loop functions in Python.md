# Collections and Loop Functions in Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Collections](#Collections)

[Loop Functions](#Loop-Functions)



## Overview

Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python's design philosophy emphasizes code readability with its notable use of significant whitespace. Its language constructs and object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming. Python is often described as a "batteries included" language due to its comprehensive standard library

Python interpreters are available for many operating systems. A global community of programmers develops and maintains CPython, an open source reference implementation. A non-profit organization, the Python Software Foundation, manages and directs resources for Python and CPython development.


## Pre-Requisites

1- Basic knowledge of any computer language

2- Pre-Installed Python

3- Pre-Installed Visual Studio Code


## Login to Azure Console

### Before you Begin

1 - All screen shots are examples ONLY. Screen shots can be enlarged by Clicking on them

2 - Every User MUST keep below credentials handy (User Name/ Login ID and Password)

3 - Do NOT use name and other data from screen shots.Only use  data(including subscription id) provided in the content section of the lab

In this section we will login to the OCI console and adjust your screen size (if needed).

**Step 1.** Sign in to your account using the below credentials 
            (Please type in your credentials):

 **login_ID:** {{login-id}} <br>
 **login_Password:** {{login-password}}<br>
 **subscription_ID:** {{subscription-ID}} <br>


**Note:** Your password should be updated automatically for you, but sometimes you may be asked to change it after signing in the first time. If prompted, please update the password. You can use this one to expedite things: Azure123Q!!!! . It will not be saved after this lab expires.


**Step 2.** Reduce the Browser Display Window Size/Resolution to fit your needs(Below example is for Chrome). 


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Getting%20started%20with%20Python/Resolution-1.png" alt="image-alt-text">


## Collections 

**Namedtuple( )**

It returns a tuple with a named entry, which means there will be a name assigned to each value in the tuple. It overcomes the problem of accessing the elements using the index values. With namedtuple( ) it becomes easier to access these values, since you do not have to remember the index values to get specific elements.

Look at the following code to understand how you can use namedtuple.

Copy the code and execute in Visual Studio Code. 


```
import collections as col
#create employee NamedTuple
Employee = col.namedtuple('Employee', ['name', 'city', 'salary'])
#Add two employees
e1 = Employee('Asim', 'Delhi', '25000')
e2 = Employee('Bibhas', 'Kolkata', '30000')
#Access the elements using index
print('The name and salary of e1: ' + e1[0] + ' and ' + e1[2])
#Access the elements using attribute name
print('The name and salary of e2: ' + e2.name + ' and ' + e2.salary)
#Access the elements using getattr()
print('The City of e1 and e2: ' + getattr(e1, 'city') + ' and ' + getattr(e2, 'city'))
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/Named%20Tuple.png" alt="image-alt-text">


**Deque**

A double-ended queue, or deque, has the feature of adding and removing elements from either end. The Deque module is a part of collections library. It has the methods for adding and removing elements which can be invoked directly with arguments.

Look at the following code to understand how you can use Deque

Copy the code and execute in Visual Studio Code. 


```
import collections
# Create a deque
DoubleEnded = collections.deque(["Mon","Tue","Wed"])
print (DoubleEnded)

# Append to the right
print("Adding to the right: ")
DoubleEnded.append("Thu")
print (DoubleEnded)

# append to the left
print("Adding to the left: ")
DoubleEnded.appendleft("Sun")
print (DoubleEnded)

# Remove from the right
print("Removing from the right: ")
DoubleEnded.pop()
print (DoubleEnded)

# Remove from the left
print("Removing from the left: ")
DoubleEnded.popleft()
print (DoubleEnded)

# Reverse the dequeue
print("Reversing the deque: ")
DoubleEnded.reverse()
print (DoubleEnded)
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/Deque.png" alt="image-alt-text">



**ChainMap**

The ChainMap is used to encapsulates the dictionaries into single unit.

The ChainMapis a standard library class, which is located in the collections module.

**Operations on ChainMap**

1- keys() :- This function is used to display all the keys of all the dictionaries in ChainMap.

2- values() :- This function is used to display values of all the dictionaries in ChainMap.

3- maps :- This function is used to display keys with corresponding values of all the dictionaries in ChainMap.

Copy the code and execute in Visual Studio Code tool.


```
import collections as col
con_code1 = {'India' : 'IN', 'China' : 'CN'}
con_code2 = {'France' : 'FR', 'United Kingdom' : 'GB'}
chain = col.ChainMap(con_code1, con_code2)
print("Initial Chain: " + str(chain.maps))
print('The keys in the ChainMap: ' + str(list(chain.keys())))
print('The values in the ChainMap: ' + str(list(chain.values())))
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/chainmap.png" alt="image-alt-text">



**Counter** 

A Counter is a container that keeps track of how many times equivalent values are added. It can be used to implement the same algorithms for which bag or multiset data structures are commonly used in other languages

Copy the code and execute in Visual Studio Code tool.


```
from collections import Counter

# empty Counter
counter = Counter()
print(counter)  # Counter()

# Counter with initial values
counter = Counter(['a', 'a', 'b'])
print(counter)  # Counter({'a': 2, 'b': 1})

counter = Counter(a=2, b=3, c=1)
print(counter)  # Counter({'b': 3, 'a': 2, 'c': 1})
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/counter.png" alt="image-alt-text">



**OrderedDict** 

The OrderedDict is a subclass of dict object in Python. The only difference between OrderedDict and dict is that, in OrderedDict, it maintains the orders of keys as inserted. In the dict, the ordering may or may not be happen.

The OrderedDict is a standard library class, which is located in the collections module.

Copy the code and execute in Visual Studio Code tool.


```
import collections
#Create normal dict
my_dict = {}
my_dict['AA'] = 11
my_dict['BB'] = 22
my_dict['CC'] = 33
my_dict['DD'] = 44
for item in my_dict.items():
   print(item)
print()
#Create ordered dict
my_ord_dict = collections.OrderedDict()
my_ord_dict['AA'] = 11
my_ord_dict['BB'] = 22
my_ord_dict['CC'] = 33
my_ord_dict['DD'] = 44
for item in my_ord_dict.items():
   print(item)
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/Orderdict.png" alt="image-alt-text">




**defaultdict**

Defaultdict is a container like dictionaries present in the module collections. Defaultdict is a sub-class of the dict class that returns a dictionary-like object.

Copy the code and execute in Visual Studio Code tool.


```
from collections import defaultdict

defaultdict_demo = defaultdict(set)

defaultdict_demo['one'].add(1)
defaultdict_demo['two'].add(2)
defaultdict_demo['one'].add('1')
defaultdict_demo['three']

print(dict(defaultdict_demo.items()))
```



Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/defaultdict.png" alt="image-alt-text">




**UserList**

This class acts like a wrapper around the list objects. It is a useful base class for other list like classes which can inherit from them and override the existing methods or even add a fewer new ones as well.

The need for this class came from the necessity to subclass directly from list. It becomes easier to work with this class as the underlying list becomes an attribute.

Copy the code and execute in Visual Studio Code tool.


```
# creating an empty list 
lst = [] 
  
# number of elemetns as input 
n = int(input("Enter number of elements : ")) 
  
# iterating till the range 
for i in range(0, n): 
    ele = int(input()) 
  
    lst.append(ele) # adding the element 
      
print(lst) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/Userlist.png" alt="image-alt-text">



## Loop Functions

**For Loop**

A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

This is less like the for keyword in other programming languages, and works more like an iterator method as found in other object-orientated programming languages.

With the for loop we can execute a set of statements, once for each item in a list, tuple, set etc.

Copy the code and execute in Visual Studio Code tool.


```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/ForLoop.png" alt="image-alt-text">



**While Loop**

While Loops is used to execute a block of statements repeatedly until a given condition is satisfied. Python uses indentation as its method of grouping statements. When a while loop is executed, expr is first evaluated in a Boolean context and if it is true, the loop body is executed.

Copy the code and execute in Visual Studio Code tool.


```
i = 1
while i < 6:
  print(i)
  i += 1
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/While%20loop.png" alt="image-alt-text">



**Nested Loop**

A nested loop is a loop that occurs within another loop, structurally similar to nested if statements.

Copy the code and execute in Visual Studio Code tool.


```
A = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
f = 1
print(A)
for i in range(0, 3):
    f *= 10
    for j in range(0, 3):
       A[i][j] *= f
print(A)
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/NestedLoop.png" alt="image-alt-text">


**The break Statement**

With the break statement we can stop the loop before it has looped through all the items:

Copy the code and execute in Visual Studio Code tool.


```
# program to display all the elements before number 88
for num in [11, 9, 88, 10, 90, 3, 19]:
   print(num)
   if(num==88):
	   print("The number 88 is found")
	   print("Terminating the loop")
	   break
```



Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/breakstatement.png" alt="image-alt-text">


**The continue Statement**

The continue statement rejects all the remaining statements in the current iteration of the loop and moves the control back to the top of the loop. The continue statement can be used in both while and for loops.

Copy the code and execute in Visual Studio Code tool.


```
# Python program to 
# demonstrate continue 
# statement 
  
# loop from 1 to 10 
for i in range(1, 11): 
  
    # If i is equals to 6,   
    # continue to next iteration   
    # without printing  
    if i == 6: 
        continue
    else: 
        # otherwise print the value 
        # of i 
        print(i, end = " ") 
```



Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/continue%20satatement.png" alt="image-alt-text">


**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.s