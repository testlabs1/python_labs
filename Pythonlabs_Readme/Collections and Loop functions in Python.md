# Heading

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Collections in Python](#Collections-in-Python)

[Demon on collections in Python](#Demo-on-collections-in-Python)

[Loop functions in Python](#Loop-functions-in-Python)

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


## Collections in Python 

**Step-1:**

**Numeric types**

Python supports the following numerical data types int, float and complex. The integer numbers (e.g. 8, 3, 120) have type int, the ones with a fractional part (e.g. 5.0, 1.6) have type float. Python also has built-in support for complex numbers and uses the j or J suffix to indicate the imaginary part (e.g. 2+7j). 

Let us see an example to understand the numeric types. 

$@@@@@@Copy the code and execute in Visual Studio Code. 


```
id=1 
avg_marks=25.6 
vec=2+3j 
print("Value of id is:",id) 
print("Value of average-marks is:",avg_marks) 
print("Value of vector is:",vec) 
```

@@@@@@@@Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Collections%20and%20Loop%20functions%20in%20Pythons/breakstatement.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-16.png" alt="image-alt-text">



<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Numeric%20Data%20types%20in%20python-1.png" alt="image-alt-text">



**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.