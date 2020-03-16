# Getting started with Python
 
[Overview](#overview)
 
[Pre-Requisites](#pre-requisites)
 
[Login to Azure Console](#login-to-azure-console)

[Regular Expression](#Regular-Expression)

[The findall() Function](#The-findal()-Function)
 
[The search() Function](#The-search()-Function)

[The spilt() Function](#The-spilt()-Function)

[The sub() Function](#The-sub()-Function)


## Overview
 
Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python's design philosophy emphasizes code readability with its notable use of significant whitespace. Its language constructs and object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.
 
Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming. Python is often described as a "batteries included" language due to its comprehensive standard library
 
Python interpreters are available for many operating systems. A global community of programmers develops and maintains CPython, an open source reference implementation. A non-profit organization, the Python Software Foundation, manages and directs resources for Python and CPython development.
 
## Pre-Requisites
 
 Basic knowledge of any computer language
 
## Login to Azure Console
 
### Before you Begin:
 
1- All screen shots are examples ONLY. Screen shots can be enlarged by Clicking on them
 
2- Every User MUST keep below credentials handy.
User Name/ Login ID
Password
 
3- Do NOT use name and other data from screen shots.Only use  data(including subscription id) provided in the content section of the lab
 
In this section we will login to the OCI console and adjust your screen size (if needed).
 
**Step 1.** Sign in to your account using the below credentials 
            (Please type in your credentials):
 
 **login_ID:** {{login-id}} <br>
 **login_Password:** {{login-password}}<br>
 **subscription_ID:** {{subscription-ID}} <br>
 
**Note:** Your password should be updated automatically for you, but sometimes you may be asked to change it after signing in the first time. If prompted, please update the password. You can use this one to expedite things: Azure123Q!!!! . It will not be saved after this lab expires.
 
**Step 2.** Reduce the Browser Display Window Size/Resolution to fit your needs(Below example is for Chrome). 
 
![](https://qloudableassets.blob.core.windows.net/devops/OCI/advanced-ansible-playbooks/images/2.jpg?st=2019-09-06T10%3A31%3A31Z&se=2022-09-07T10%3A31%3A00Z&sp=rl&sv=2018-03-28&sr=c&sig=fwljWymO6LKz5xubtKh3mAsK3r858hNP%2Bl6%2FtadP4MM%3D)
 
# Regular Expression

A regular expression is a special sequence of characters that helps you match or find other strings or sets of strings, using a specialized syntax held in a pattern. Regular expressions are widely used in UNIX world. The Python module re provides full support for Perl-like regular expressions in Python.

A Regular Expression (RegEx) is a sequence of characters that defines a search pattern. For example,

^a...s$

The above code defines a RegEx pattern. The pattern is: any five letter string starting with a and ending with s.

## Example RegEX. exmaple program.

Search the string to see if it starts with "The" and ends with "Spain":

import re

#Check if the string starts with "The" and ends with "Spain":

txt = "The rain in Spain"
x = re.search("^The.*Spain$", txt)

if (x):
  print("YES! We have a match!")
else:
  print("No match")

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx2.png" alt="image-alt-text">

# RegEx Functions
The re module offers a set of functions that allows us to search a string for a match.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx3.png" alt="image-alt-text">

# Metacharacters
Metacharacters are characters with a special meaning.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx4.png" alt="image-alt-text">

# Special Sequences
A special sequence is a \ followed by one of the characters in the list below, and has a special meaning.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx6.png" alt="image-alt-text">

# Sets
A set is a set of characters inside a pair of square brackets [] with a special meaning.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx5.png" alt="image-alt-text">


# The findall() Function

The findall() function returns a list containing all matches.

## Example
Print a list of all matches

import re

#Return a list containing every occurrence of "ai":

txt = "The rain in Spain"
x = re.findall("ai", txt)
print(x)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc%27s/RegEx7.png" alt="image-alt-text">

The list contains the matches in the order they are found If no matches are found, an empty list is returned.

## Example

Return an empty list if no match was found.

import re

txt = "The rain in Spain"

#Check if "Portugal" is in the string:

x = re.findall("Portugal", txt)
print(x)

if (x):
  print("Yes, there is at least one match!")
else:
  print("No match")

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx8.png" alt="image-alt-text">

# The search() Function
The search() function searches the string for a match, and returns a Match object if there is a match.If there is more than one match, only the first occurrence of the match will be returned

## Example
Search for the first white-space character in the string.

import re

txt = "The rain in Spain"
x = re.search("\s", txt)

print("The first white-space character is located in position:", x.start()) 

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx9.png" alt="image-alt-text">

If no matches are found, the value None is returned.

import re

txt = "The rain in Spain"
x = re.search("Portugal", txt)
print(x)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx10.png" alt="image-alt-text">

# The spilt() Function

The split() function returns a list where the string has been split at each match.

import re

#Split the string at every white-space character:

txt = "The rain in Spain"
x = re.split("\s", txt)
print(x)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx11.png" alt="image-alt-text">

# The sub() Function
The sub() function replaces the matches with the text of your choice.

import re

#Replace all white-space characters with the digit "9":

txt = "The rain in Spain"
x = re.sub("\s", "9", txt)
print(x)

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx12.png" alt="image-alt-text">


The Match object has properties and methods used to retrieve information about the search, and the result:

.span() returns a tuple containing the start-, and end positions of the match.
.string returns the string passed into the function
.group() returns the part of the string where there was a match

## Example
Print the position (start- and end-position) of the first match occurrence.

The regular expression looks for any words that starts with an upper case "S"

import re

#Search for an upper case "S" character in the beginning of a word, and print its position:

txt = "The rain in Spain"
x = re.search(r"\bS\w+", txt)
print(x.span())

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx13.png" alt="image-alt-text">

Example
Print the string passed into the function.

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx14.png" alt="image-alt-text">

## Example
Print the part of the string where there was a match.

The regular expression looks for any words that starts with an upper case "S"

import re

#Search for an upper case "S" character in the beginning of a word, and print the word:

txt = "The rain in Spain"
x = re.search(r"\bS\w+", txt)
print(x.group())

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Regulations%20Expressions%20Img%20Doc's/RegEx15.png" alt="image-alt-text">


**Tip:** We suggest you to keep save your file in Auto save mode to save it automatically.

**Note:** You can use your preferred IDE/ text editor to write the code. In this course Visual Studio Code will be used to write and execute the Python programs. 
Copy the following code and paste it in the Visual Studio Code and save the file with Demo.py name. 


## Python program to print output on the screen 

Copy the below command and paste it into the Visual Studio Code

```
print("Hello Python")
```

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-8.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-10.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-11.png" alt="image-alt-text">