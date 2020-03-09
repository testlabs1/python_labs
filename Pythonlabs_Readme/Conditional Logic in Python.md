# Conditional Logic in Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Conditional Logic](#Conditional-Logic)

[Handling Multiple Conditions](#Handling-Multiple-Conditions)

[Complex Conditions](#Complex-Conditions)



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


## Conditional Logic

Conditional Statement in Python perform different computations or actions depending on whether a specific Boolean constraint evaluates to true or false. Conditional statements are handled by IF statements in Python.

Python supports the usual logical conditions from mathematics:

-	Equals: a == b
-	Not Equals: a != b
-	Less than: a < b
-	Less than or equal to: a <= b
-	Greater than: a > b
-	Greater than or equal to: a >= b

These conditions can be used in several ways, most commonly in "if statements" and loops.

**If statement:**

An "**if** statement" is written by using the if keyword.

Copy the code and execute in Visual Studio Code tool.


```
a = 33
b = 200
if b > a:
  print("b is greater than a")
```

In this example we use two variables, a and b, which are used as part of the if statement to test whether b is greater than a. As a is 33, and b is 200, we know that 200 is greater than 33, and so we print to screen that "b is greater than a".

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/If-1.png" alt="image-alt-text">



**Indentation**

Python relies on indentation (whitespace at the beginning of a line) to define scope in the code. Other programming languages often use curly-brackets for this purpose.

If statement, without indentation (will raise an error)

Copy the code and execute in Visual Studio Code tool.


```
a = 33
b = 200
if b > a:
print("b is greater than a") # you will get an error
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/If%20with%20error-1.png" alt="image-alt-text">


**Elif**

The **elif** keyword is pythons way of saying "if the previous conditions were not true, then try this condition".

Copy the code and execute in Visual Studio Code tool.


```
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```


In this example a is equal to b, so the first condition is not true, but the elif condition is true, so we print to screen that "a and b are equal".

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Elif-1.png" alt="image-alt-text">


**Else**

The **else** keyword catches anything which isn't caught by the preceding conditions.

**Step-1:** You can also have an **else** with the **elif**

Copy the code and execute in Visual Studio Code tool.


```
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```


In this example a is greater than b, so the first condition is not true, also the elif condition is not true, so we go to the else condition and print to screen that "a is greater than b".

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Elif%20and%20Else-1.png" alt="image-alt-text">


**Step-2:** You can also have an **else** without the **elif**

Copy the code and execute in Visual Studio Code tool.


```
a = 200
b = 33
if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Else%20wihtout%20Elif-1.png" alt="image-alt-text">


**Shorthand If**

If you have only one statement to execute, you can put it on the same line as the **if** statement.
One line **if** statement:

Copy the code and execute in Visual Studio Code tool.


```
if a > b: print("a is greater than b")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Shorthand%20If-1.png" alt="image-alt-text">


## Handling Multiple Conditions

**Shorthand If ... Else**

**One line if else statement:**

If you have only one statement to execute, one for **if**, and one for **else**, you can put it all on the same line.

Copy the code and execute in Visual Studio Code tool.


```
a = 2
b = 330
print("A") if a > b else print("B")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Shorthand%20If%20Else-1.png" alt="image-alt-text">


**One line if else statement, with 3 conditions:**

You can also have multiple **else** statements on the same line.

Copy the code and execute in Visual Studio Code tool.


```
a = 330
b = 330
print("A") if a > b else print("=") if a == b else print("B")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Shorthand%20If%20Else%20with%203%20Conditions-1.png" alt="image-alt-text">


## Complex Conditions

**And**

The **and** keyword is a logical operator, and is used to combine conditional statements.

Test if a is greater than b, **AND** if c is greater than a

Copy the code and execute in Visual Studio Code tool.


```
a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/And-1.png" alt="image-alt-text">


**Or**

The **or** keyword is a logical operator, and is used to combine conditional statements.

Test if a is greater than b, **OR** if a is greater than c

Copy the code and execute in Visual Studio Code tool.


```
a = 200
b = 33
c = 500
if a > b or a > c:
  print("At least one of the conditions is True")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Or-1.png" alt="image-alt-text">


**Nested If**

You can have **if** statements inside **if** statements, this is called Nested if statements.

Copy the code and execute in Visual Studio Code tool.


```
x = 41

if x > 10:
  print("Above ten,")
  if x > 20:
    print("and also above 20!")
  else:
    print("but not above 20.")
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/Nested%20If-1.png" alt="image-alt-text">


**The pass Statement**

if statements cannot be empty, but if you for some reason have an **if** statement with no content, put in the **pass** statement to avoid getting an error.

Copy the code and execute in Visual Studio Code tool.


```
a = 33
b = 200

if b > a:
  pass
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Conditional%20Logic%20in%20Python/The%20Pass%20Statement-1.png" alt="image-alt-text">



**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.