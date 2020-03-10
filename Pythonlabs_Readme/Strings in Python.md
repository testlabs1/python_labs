# Getting started with Python

## Table of Contents

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Strings Concept](#Strings-Concept)

[Formatting Strings in Python](#Formatting-Strings-in-Python)



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


## Strings concept

You can produce output using print () function in Python. You can pass multiple expressions by separating them with commas, all these the expressions are converted to strings by print () function before writing them to the screen. 
Syntax: print(value(s), sep= ‘ ‘, end = ‘\n’, file=file, flush=flush) 
Let see an example to output a message, for this let us create a file called demo.py in the Visual Studio Code and run code as shown below. 

## What is strings

A string in Python is a sequence of characters. It is a derived data type. Strings are immutable. This means that once defined, they cannot be changed. Many Python methods, such as replace(), join(), or split() modify strings. However, they do not modify the original string. They create a copy of a string which they modify and return to the caller.

## Creating a String

Strings in Python can be created using single quotes or double quotes or even triple quotes.

# Python Program for String Creation 
  
# Creating a String with single Quotes 
String1 = 'Welcome to the Geeks World'

print("String with the use of Single Quotes: ") 

print(String1)
  
<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Strings%20single%20quotes.png" alt="image-alt-text">

# Creating a String with double Quotes 
String1 = "I'm a Geek"
print("\nString with the use of Double Quotes: ") 
print(String1) 

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Strings%20with%20double%20quotes.png" alt="image-alt-text">
  
# Creating a String with triple Quotes 
String1 = '''I'm a Geek and I live in a world of "Geeks"'''
print("\nString with the use of Triple Quotes: ") 
print(String1) 

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Strings%20with%20triple%20quotes.png" alt="image-alt-text">
  
# Creating String with triple Quotes allows multiple lines 
String1 = '''Geeks 
            For 
            Life'''
print("\nCreating a multiline String: ") 
print(String1)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Creating%20a%20multiline%20String.png" alt="image-alt-text">

## Accessing characters in Python

In Python, individual characters of a String can be accessed by using the method of Indexing. Indexing allows negative address references to access characters from the back of the String, e.g. -1 refers to the last character, -2 refers to the second last character and so on.
While accessing an index out of the range will cause an IndexError. Only Integers are allowed to be passed as an index, float or other types will cause a TypeError.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Accessing%20characters%20in%20Python.png" alt="image-alt-text">

# Python Program to Access characters of String 
  
String1 = "GeeksForGeeks"
print("Initial String: ") 
print(String1) 
  
# Printing First character 
print("\nFirst character of String is: ") 
print(String1[0]) 
  
# Printing Last character 
print("\nLast character of String is: ") 
print(String1[-1])

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Accessing%20Characters%20in%20Python2.png" alt="image-alt-text">


## String Slicing

To access a range of characters in the String, method of slicing is used. Slicing in a String is done by using a Slicing operator (colon).

# Python Program to demonstrate String slicing 
  
# Creating a String 
String1 = "GeeksForGeeks"
print("Initial String: ")  
print(String1) 
  
# Printing 3rd to 12th character 
print("\nSlicing characters from 3-12: ") 
print(String1[3:12]) 
  
# Printing characters between 3rd and 2nd last character 

print("\nSlicing characters between " +
    "3rd and 2nd last character: ") 
print(String1[3:-2])

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/String%20Slicing.png" alt="image-alt-text">

## Formatting Strings In Python

String Formatting. Python uses C-style string formatting to create new, formatted strings. The "%" operator is used to format a set of variables enclosed in a "tuple" (a fixed size list), together with a format string, which contains normal text together with "argument specifiers", special symbols like "%s" and "%d".

Let's say you have a variable called "name" with your user name in it, and you would then like to print

# This prints out "Hello, John!"
name = "John"
print("Hello, %s!" % name)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Formatting%20Strings%20in%20Python.png" alt="image-alt-text">

To use two or more argument specifiers, use a tuple (parentheses):

# This prints out "John is 23 years old."
name = "John"
age = 23
print("%s is %d years old." % (name, age))

<img src ="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Formatting%20strings%20in%20python2.png" alt="image-alt-text">

Try to fix the code to print out the correct information by changing the string.

s = "Hey there! what should this string be?"
# Length should be 20
print("Length of s = %d" % len(s))

# First occurrence of "a" should be at index 8
print("The first occurrence of the letter a = %d" % s.index("a"))

# Number of a's should be 2
print("a occurs %d times" % s.count("a"))

# Slicing the string into bits
print("The first five characters are '%s'" % s[:5]) # Start to 5
print("The next five characters are '%s'" % s[5:10]) # 5 to 10
print("The thirteenth character is '%s'" % s[12]) # Just number 12
print("The characters with odd index are '%s'" %s[1::2]) #(0-based indexing)
print("The last five characters are '%s'" % s[-5:]) # 5th-from-last to end

# Convert everything to uppercase
print("String in uppercase: %s" % s.upper())

# Convert everything to lowercase
print("String in lowercase: %s" % s.lower())

# Check how a string starts
if s.startswith("Str"):
    print("String starts with 'Str'. Good!")

# Check how a string ends
if s.endswith("ome!"):
    print("String ends with 'ome!'. Good!")

# Split the string into three separate strings,
# each containing only a word
print("Split the words of the string: %s" % s.split(" "))

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Strings%20in%20Python/Formatting%20Strings%20in%20Python3.png" alt="image-alt-text">


**Tip:** We suggest you to keep save your file in Auto save mode to save it automatically.

**Note:** You can use your preferred IDE/ text editor to write the code. In this course Visual Studio Code will be used to write and execute the Python programs. 
Copy the following code and paste it in the Visual Studio Code and save the file with Demo.py name. 


### Python program to print output on the screen 

Copy the below command and paste it into the Visual Studio Code

```
print("Hello Python")
```

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-8.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-10.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-11.png" alt="image-alt-text">