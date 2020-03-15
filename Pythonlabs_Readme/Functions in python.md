#  Functions in Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Functions](#Functions)


## Overview

Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python's design philosophy emphasizes code readability with its notable use of significant whitespace. Its language constructs and object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming. Python is often described as a "batteries included" language due to its comprehensive standard library

Python interpreters are available for many operating systems. A global community of programmers develops and maintains CPython, an open source reference implementation. A non-profit organization, the Python Software Foundation, manages and directs resources for Python and CPython development.


## Pre-Requisites

Basic knowledge of any computer language


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


## Functions in Python

**Function()**
function is a group of related statements that perform a specific task.
Functions help break our program into smaller and modular chunks. As our program grows larger and larger, functions make it more organized and manageable.



```
def my_function():
  print("Hello from a function")

my_function()

```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Functions.png" alt="image-alt-text">


## Arguments and Types of Arguments

**Arguments()**
In Python, you can define a function that takes variable number of arguments. You will learn to define such functions using default, keyword and arbitrary arguments in this article.

**Types of Arguments()**

**Arbitrary Arguments()**

Arguments Python allows us to handle this kind of situation through function calls with arbitrary number of arguments. In the function definition we use an asterisk (*) before the parameter name to denote this kind of argument. 

```
def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus") 
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Arbitary%20function.png" alt="image-alt-text">


**Arbitrary Keyword Arguments()** 

Embrace keyword arguments in Python Consider using the * operator to require those arguments be specified as keyword arguments. And remember that you can accept arbitrary keyword arguments to the functions you define and pass arbitrary keyword arguments to the functions you call by using the ** operator.


```
def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus") 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.



<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Arbitarykeyword.png" alt="image-alt-text">


**Keyword Arguments()**

Keyword Arguments Python allows functions to be called using keyword arguments. When we call functions in this way, the order (position) of the arguments can be changed.

```
def my_function(child3, child2, child1):
  print("The youngest child is " + child3)

my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus") 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Keywordfunction.png" alt="image-alt-text">


**Default Parameter Value()**

Python has a different way of representing syntax and default values for function arguments. Default values indicate that the function argument will take that value if no argument value is passed during function call.


```
def my_function(country = "Norway"):
  print("I am from " + country)

my_function("Sweden")
my_function("India")
my_function()
my_function("Brazil") 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Defualtfunction.png" alt="image-alt-text">

**Passing List in an Argument()**

If we pass a list to a function, we have to consider two cases: Elements of a list can be changed in place where actually passes a reference to the list, not a copy of the list. 


```
def my_function(food):
  for x in food:
    print(x)

fruits = ["apple", "banana", "cherry"]

my_function(fruits)
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/passingfunction.png" alt="image-alt-text">


**Return Values()**
A return statement ends the execution of the function call and "returns" the result, i.e. the value of the expression following the return keyword, to the caller. If the return statement is without an expression, the special value None is returned.

```
def my_function(x):
  return 5 * x

print(my_function(3))
print(my_function(5))
print(my_function(9)) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Returnfunction.png" alt="image-alt-text">


**Anonymous Function ()**
Anonymous function is a function that is defined without a name. While normal functions are defined using the def keyword, in Python anonymous functions are defined using the lambda keyword. Hence, anonymous functions are also called lambda functions.


```
def square(x):
    return x * x
f_square = lambda x: x * x
print(square(10))  # 100
print(f_square(10))  # 100
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Anonymousfunction.png"  alt="image-alt-text">


**Recursive Functions in Python()**
A recursive function is a function defined in terms of itself via self-referential expressions. This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.


```
def fibonacci_numbers_at_index(count):
    if count <= 1:
        return count
    else:
        return fibonacci_numbers_at_index(count - 1) + fibonacci_numbers_at_index(count - 2)


count = 5
i = 1
while i <= count:
    print(fibonacci_numbers_at_index(i))
    i += 1
    
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Functions%20in%20Pythons/Recursivefunction.png" alt="image-alt-text">


**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.
