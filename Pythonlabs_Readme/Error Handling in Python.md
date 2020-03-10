# Error Handling in Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Exception Handling](#Exception-Handling)

[Many Exceptions](#Many-Exceptions)

[Else](#Else)

[Finally](#Finally)

[Raise An Exception](#Raise-An-Exception)


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


## Exception Handling

When an error occurs, or exception as we call it, Python will normally stop and generate an error message.

**Step-1:** This statement will raise an error, because x is not defined.

Copy the code and execute in Visual Studio Code tool.

```
print(x)
``` 

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Error-1.png" alt="image-alt-text">


**Step-2:** These exceptions can be handled using the try statement. The try block will generate an exception, because x is not defined.

Copy the code and execute in Visual Studio Code tool.

```
try:
  print(x)
except:
  print("An exception occurred")
``` 

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Try%20and%20Except-1.png" alt="image-alt-text">

Since the try block raises an error, the except block will be executed. Without the try block, the program will crash and raise an error

## Many Exceptions

You can define as many exception blocks as you want, e.g. if you want to execute a special block of code for a special kind of error.

Print one message if the try block raises a NameError and another for other errors.

Copy the code and execute in Visual Studio Code tool.

```
try:
  print(x)
except NameError:
  print("Variable x is not defined")
except:
  print("Something else went wrong")
```
Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Many%20Exceptions-1.png" alt="image-alt-text">

## Else

You can use the else keyword to define a block of code to be executed if no errors were raised.
In this example, the try block does not generate any error.

Copy the code and execute in Visual Studio Code tool.

```
try:
  print("Hello")
except:
  print("Something went wrong")
else:
  print("Nothing went wrong")
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Else-1.png" alt="image-alt-text">

## Finally

**Step-1:**

The finally block, if specified, will be executed regardless if the try block raises an error or not.

Copy the code and execute in Visual Studio Code tool.

```
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Finally-1.png" alt="image-alt-text">

**Step-2:**

This can be useful to close objects and clean up resources. Try to open and write to a file that is not writable.

Copy the code and execute in Visual Studio Code tool.

```
try:
  f = open("demofile.txt")
  f.write("Lorum Ipsum")
except:
  print("Something went wrong when writing to the file")
finally:
  f.close()
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Finally-2.png" alt="image-alt-text">


The program can continue, without leaving the file object open.

## Raise An Exception

As a Python developer you can choose to throw an exception if a condition occurs. To throw (or raise) an exception, use the raise keyword.

**Step-1:**

Raise an error and stop the program if x is lower than 0.

Copy the code and execute in Visual Studio Code tool.

```
x = -1

if x < 0:
  raise Exception("Sorry, no numbers below zero")
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Raise-1.png" alt="image-alt-text">

The raise keyword is used to raise an exception.
You can define what kind of error to raise, and the text to print to the user.

**Step-2:**

Raise a TypeError if x is not an integer.
Copy the code and execute in Visual Studio Code tool.

```
x = "hello"

if not type(x) is int:
  raise TypeError("Only integers are allowed")
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Error%20handling%20in%20Python/Raise-2.png" alt="image-alt-text">


**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.