# Getting started with Python

## Table of Contents

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

### Before you Begin

1 - All screen shots are examples ONLY. Screen shots can be enlarged by Clicking on them

2 - Every User MUST keep below credentials handy.
        User Name/ Login ID
        Password

3 - Do NOT use name and other data from screen shots.Only use  data(including subscription id) provided in the content section of the lab

In this section we will login to the OCI console and adjust your screen size (if needed).

**Step 1.** Sign in to your account using the below credentials 
            (Please type in your credentials):

 **login_ID:** {{login-id}} <br>
 **login_Password:** {{login-password}}<br>
 **subscription_ID:** {{subscription-ID}} <br>


**Note:** Your password should be updated automatically for you, but sometimes you may be asked to change it after signing in the first time. If prompted, please update the password. You can use this one to expedite things: Azure123Q!!!! . It will not be saved after this lab expires.


**Step 2.** Reduce the Browser Display Window Size/Resolution to fit your needs(Below example is for Chrome). 

<img src="https://github.com/testlabs1/python_labs/blob/master/Pythonlabs_Images/Getting%20started%20with%20Python/Resolution-1.png?raw=true" alt="image-alt-text">


## Installing Python

For installing Python we need to download the software from the python website. Copy below URL and paste it into Chrome and download latest version.

```
https://www.python.org/downloads/
```

Follow the images for steps to install python.

**Step-1.** Double click on the Python 3.x.x setup and select Customize installation.
 
<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-1.png" alt="image-alt-text">


**Step-2.** Select the installation files to be save path from Browse button

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-2.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-3.png" alt="image-alt-text">


**Note:** We need to add the installed software path in Environment variables for that follow the steps.


**Step-3.** Right click on This PC Icon and select properties there after you can see left side of the opened window click on the Advanced system settings.


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-4.png" alt="image-alt-text">


**Step-4.** Select the Environment variables and Edit it.

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-5.png" alt="image-alt-text">
 

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-6.png" alt="image-alt-text">


**Step-5.** Paste the installed software path by selecting New and select the OK.
   
<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-7.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-8.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-9.png" alt="image-alt-text">


### Using Windows PowerShell 

Open Windows PowerShell (Admin) in Windows 10, type SystemPropertiesAdvanced and click Enter to immediately open the System Properties

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/Install-10.png" alt="image-alt-text">


## Configuring Visual Studio Code for Python

Visual Studio Code can be available in the Apps. 

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC.png" alt="image-alt-text">


After opening the Visual Studio Code, we need to configure the python to Visual Studio Code. Follow the below steps to complete the setup.


**Step-1.** Select the Extensions from the left side of the Visual Studio Code and search for the Python.
 
<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-2.png" alt="image-alt-text">


**Step-2.** Select the Python and install it.

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-3.png" alt="image-alt-text">


**Step-3.** Go to File, select Preferences and then select Settings.

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-4.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-5.png" alt="image-alt-text">


**Step-4.** Select the search bar and type the PythonPath and then select paste the python installed path.

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-6.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-7.png" alt="image-alt-text">


**Step-5.** Install the pylint while executing the program (for the first time of python lab creation).

**Step-6.** Install or create the json code for automating debugging.

<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-12.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-13.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-14.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-15.png" alt="image-alt-text">


## Using print function Comments in Python

You can produce output using print () function in Python. You can pass multiple expressions by separating them with commas, all these the expressions are converted to strings by print () function before writing them to the screen. 
Syntax: print(value(s), sep= ‘ ‘, end = ‘\n’, file=file, flush=flush) 
Let see an example to output a message, for this let us create a file called demo.py in the Visual Studio Code and run code as shown below. 


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


Click Run button (highlighted in blue color at topmost right) to run the Python file in terminal. Once the program runs successfully you will get the output at the bottom (highlighted in blue color) as shown below. 


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-12.png" alt="image-alt-text">


<img src="https://raw.githubusercontent.com/testlabs1/python_labs/master/Pythonlabs_Images/Getting%20started%20with%20Python/VSC-15.png" alt="image-alt-text">
 

**Note:**<br>
In this lab Python 3.x is used for demonstrating the different concepts in Python. Please make sure you are using the right version while executing demos. 

You have successfully completed this tutorial. In this Training lab we have learnt Python program to print output on the screen in Azure. We have learnt on how to Python, How Python connects with Visual Studio Code.