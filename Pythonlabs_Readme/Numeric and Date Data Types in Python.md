# Getting started with Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Numerical Data Types in Python](#Numerical-Data-Types-in-Python)

[Date in Python](#Date-in-Python)


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

## Numerical Data Types in Python 

**Step-1:**

**Numeric types**

Python supports the following numerical data types int, float and complex. The integer numbers (e.g. 8, 3, 120) have type int, the ones with a fractional part (e.g. 5.0, 1.6) have type float. Python also has built-in support for complex numbers and uses the j or J suffix to indicate the imaginary part (e.g. 2+7j). 

Let us see an example to understand the numeric types. 

Copy the code and execute in Visual Studio Code. 


```
id=1 
avg_marks=25.6 
vec=2+3j 
print("Value of id is:",id) 
print("Value of average-marks is:",avg_marks) 
print("Value of vector is:",vec) 
```

Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-12.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-16.png" alt="image-alt-text">



<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Numeric%20Data%20types%20in%20python-1.png" alt="image-alt-text">


**Step-2:** 

**Different operations on numbers**

Python supports most of the operators on numbers for example for addition (+), subtraction (-), mortification (*), division (/) and for power(**). Division (/) always returns a float. To do floor division and get an integer result (discarding any fractional result) you can use the // operator; to calculate the remainder you can use %. 

The following example demonstrate the different operations on numbers. 

Copy the code and execute in Visual Studio Code. 

```
num1=23 
num2=2 
num3=27.4 
print("Addition of num1 and num2 is :",num1+num2) 
print("Addition of num1 and num3 is :",num1+num3) 
print("power of number is:",num1**num2) 
print("Division of num1 and num2 is:",num1/num2) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Numeric%20Data%20types%20in%20python-2.png" alt="image-alt-text">


**Step-3:**

**Type Conversion**

Sometimes you need to convert from one type to another. Python support type conversation using int (), float () and complex () methods. 

The following example demonstrate the conversion from string to int using int () method. 

Copy the code and execute in Visual Studio Code. 


```
num_of_items=input("Enter the number of items\n") 
price=input("Enter the price of each item\n") 
Total=int(num_of_items)*int(price) 
print("Total price is:",Total) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Numeric%20Data%20types%20in%20python-3.png" alt="image-alt-text">


## Date in Python 

**Step-1:**

**Date and Time in python**


To work with dates as date objects we can import datetime module in Python. A date in Python is not data type of its own. 
 
The following program shows how to use datetime module in Python. 

Copy the code and execute in Visual Studio Code tool. 


```
from datetime import datetime,date 
today=date.today() 
current_date_time=datetime.now() 
print ("Today's date is:" + str(today)) 
print ("Today's date and time is:" + str(current_date_time)) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Date%20Data%20types%20in%20python-1.png" alt="image-alt-text">


**Step-2:**

**Different time functions**

In Python, date, time and datetime classes provides several functions to deal with dates, times and time intervals. Date and datetime are an object in Python, so when you manipulate them, you are manipulating objects and not string or timestamps. Whenever you manipulate dates or time, you need to import datetime function. 
The datetime classes in Python are categorized into main 5 classes. 
- date – Manipulate just date (Month, day, year) 
- time – Time independent of the day (Hour, minute, second, microsecond) 
- datetime – Combination of time and date (Month, day, year, hour, second, microsecond) 
- timedelta— A duration of time used for manipulating dates 
 
The following program demonstrates different time functions. 

Copy the code in Visual Studio Code and execute it. 


```
from  datetime import datetime,date,timedelta 
today=date.today() 
twodays=timedelta(days=2) 
day_before_yesterday=today - twodays 
day=["Monday","Tuesday","Wednesday","Thursday","Friday","Saturday","Sunday"] 
print ("Today's date is:" + str(today)) 
print ("Day before yesterday day is:",day_before_yesterday) 
print ("Todays day is: "+day[(date.weekday(today))]) 
print ("Day before yesterday is: "+day[(date.weekday(day_before_yesterday))]) 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Date%20Data%20types%20in%20python-2.png" alt="image-alt-text">


**Step-3:**

**Date format**

The way date and time is represented may be different in different places, organizations etc. 
Python has strftime() and strptime() methods to handle the date format. 
The strptime() method creates a datetime object from a given string (representing date and time). 
The strptime() method takes two arguments: 
- a string representing date and time 
- format code equivalent to the first argument 
By the way, %d, %B and %Y format codes are used for day, month (full name) and year respectively 

The following example demonstrate the use of strptime() method. 

Copy the code and execute it in Visual Studio Code as shown below. 


``` 
from datetime import datetime,date 
joining_date=input("Enter you joining date in Day Month,Year(ex: 16 June, 1985) format\n") 
print("Joining_date =", joining_date) 
today = date.today()  
date_object = datetime.strptime(joining_date, "%d %B, %Y") 
years=int(today.year)-int(date_object.year) 
print("Your Total Experience is near to : "+str(years)+" Years") 
```


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal.


<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Numeric%20and%20Date%20Data%20Types%20in%20Python/Date%20Data%20types%20in%20python-3.png" alt="image-alt-text">


**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.