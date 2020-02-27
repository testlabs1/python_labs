# Getting started with Python

[Overview](#overview)

[Pre-Requisites](#pre-requisites)

[Login to Azure Console](#login-to-azure-console)

[Installing Python](#Installing-Python)

[Configuring Visual Studio Code for Python](#Configuring-Visual-Studio-Code-for-Python)

[Using print function Comments in Python](#Using-print-function-Comments-in-Python)

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

## Installing Python

For installing Python we need to download the software from the python website. Copy below URL and paste it into Chrome and download latest version.

```https://www.python.org/downloads/```

Follow the images for steps to install python.





## Configuring Visual Studio Code for Python

Step-1: Select the Extentions from the left side of the Visual Studio Code and search for the Python.



Step-2: Select the Python and install it.



Step-3: Go to File and select Preferences and then select Settings.



Step-4: Select the search bar and type the PythonPath and then select paste the python installed path.



Step-5: Install the pylint while executing the program (for the first time of python lab creation).



Step-6: Install or create the json code for automating debugging.



## Print Output in Python

You can produce output using print () function in Python. You can pass multiple expressions by separating them with commas, all these the expressions are converted to strings by print () function before writing them to the screen. 
Syntax: print(value(s), sep= ‘ ‘, end = ‘\n’, file=file, flush=flush) 
Let see an example to output a message, for this let us create a file called demo.py in the Visual Studio Code and run code as shown below. 
Note: You can use your preferred IDE/ text editor to write the code. In this course Visual Studio Code will be used to write and execute the Python programs. 
Copy the following code and paste it in the Visual Studio Code and save the file with Demo.py name. 

### Python program to print output on the screen 

Copy the below command and paste it into the Visual Studio Code

```print("Hello Python")```

Click Run button (highlighted in blue color at top most right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 
  
**Note:**<br>

In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 


You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.
