# Setting up your system for data science - The Python Version

> Please Note: This guide makes use of Windows OS. 

## Table of contents
### Introduction



## Introduction
Data science is the trending thing in the world. Even people without computer background is trying to get familiar with data science or are trying to get hands on experience in data science. Setting your system for data science is one of the challenges most of the beginners face. They either dont know what all softwares to install,how to install and how to configure the system for data science.This guide will explain you on how to configure your system for data science. In this guide you will understand, how to install python and its dependencies for datascience.

## Getting Started
First let us figure out what all we require

#### The first thing
`Python`

Now obviously you will think which version to install? I always use two version lower to the present version.
Say if current version of python is `3.6.x` then I suggest you to install `3.4.x`
But why? You will be wondering why should you install two versions lower,right? Ok I will tell you the reason.
We will require many `python dependencies` (In simple words, the pakages we install along with python to acheieve our tasks. Like to plot a graph,we can install `matplotlib` library)to be installed along with python. Not all these packages are provided by python. So we need to get it from the respective developers. So what happens if yo install the latest version of python? Well, you will find it difficult to get a package which is compactible with the latest version of python. But packages for older versions will be available. So it is better to install 2 versions lower.

> Please Note : Python is preinstalled in Ubuntu. Just open the terminal and type `python` and press `enter` key to check.

Now [download](https://www.python.org/downloads/) python by going to official python website. Select the version and you can navigate to the bottom of the page where you can see the installation files for download. Download and install as you install any software. Usually python will be installed in C Drive. The path will be like this : `C:\Python34`,
Which will be different for you based on your installation directory. (In general, C:\PythonXX : here XX will be your version.In my case its 34 which corresponds to version 3.4)

Read more about python [here](https://www.python.org/)

To Download Python go [here](https://www.python.org/downloads/)

For Python documentation go [here](https://www.python.org/doc/)

Read about python in wikipedia go [here](https://en.wikipedia.org/wiki/Python_(programming_language))

> Inorder to run python from anywhere in your system, just by typing `python` in `command prompt`, we have to set the `path variable`.
For that Goto `My computer` -> `right click` -> Select `Advanced system Settings` -> In the new window appearing, select `Environement Variables` -> select `NEW` -> Give `Variale name` as `pythonpath` and `Variable value` as `C:\PythonXX;` (replace XX with your python version) -> `click Ok` -> `click Ok` -> `click Ok` . Similarly you can give subfolders(C:\PythonXX\Lib;C:\PythonXX\Scripts;) in that directory if you wish but not recommended. Please seperate each entry using semicolon.

> To check whether the installation and path setting is correctly done, goto `Command prompt` (Winkey + R -> Type `cmd` and press enter)
Now in command prompt type `python` and press enter. You should see something like this 

`C:\Users\username>python
Python 3.4.4 (v3.4.4:737efcadf5a6, Dec 20 2015, 20:20:57) [MSC v.1600 64 bit (AM
D64)] on win32`
`Type "help", "copyright", "credits" or "license" for more information. >>>` 

If you see this congrats.. Python is properly configured. Else go back and check your environment variable setting.

#### Installing dependencies(packages)
Dependencies are other packages or libraries which work in conjunction with python to perform some tasks. For data science there are some packages available. We can install that one by one.

Usually most of the packages are installed using `pip command`, like `pip install packagename` 
pip is a package management system used to install and manage software packages written in Python. Many packages can be found in the Python Package Index. Python 2.7.9 and later, and Python 3.4 and later include pip by default.[Read more](https://en.wikipedia.org/wiki/Pip_(package_manager))
pip is located at `C:\Python34\Scripts`

>It is a good idea to add pip to environment variable as we did for python. Just add `C:\Python34\Scripts`to `pythonpath` environment variable we made. So after this `pip install packagename` will work directly from command prompt. Else you need to navigate to `C:\Python34\Scripts`in cmd and use pip install.

>Please note if you are behind a corporate firewall you can use `pip` commands in this way `pip --proxy=yourproxyaddress install packagename`. Here replace `yourproxyaddress` with proxy your firewall is using(ask for this to your IT people) and packagename with the desired package name (package for python version you have installed in your system has to be installed)

##### Now lets see the necessary packages

###### Pandas
Pandas is a software library written for the Python programming language for data manipulation and analysis
Official [website](https://pandas.pydata.org/) |
[Wikipedia](https://en.wikipedia.org/wiki/Pandas_(software))

Install pandas : Open command prompt type `pip install pandas` press enter

###### Scipy
SciPy is an open source Python library used for scientific computing and technical computing. SciPy contains modules for optimization, linear algebra, integration, interpolation, special functions, FFT, signal and image processing, ODE solvers and other tasks common in science and engineering. 
Official [website](https://www.scipy.org/) |
[Wikipedia](https://en.wikipedia.org/wiki/SciPy)

Install pandas : Open command prompt type `pip install scipy` press enter

###### Numpy
NumPy is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.
Official [website](www.numpy.org/) |
[Wikipedia](https://en.wikipedia.org/wiki/NumPy)

Install Numpy : Open command prompt type `pip install numpy` press enter

###### Scikit-Learn
Scikit-learn (formerly scikits.learn) is a free software machine learning library for the Python programming language. It features various classification, regression and clustering algorithms including support vector machines, random forests, gradient boosting, k-means and DBSCAN
Official [website](www.scikit-learn.org) |
[Wikipedia](https://en.wikipedia.org/wiki/Scikit-learn)

Install scikitlearn : Open command prompt type `pip install scikit-learn` press enter

>Scikit-learn requires:
NumPy,
SciPy


###### Matplotlib
Matplotlib is a plotting library for the Python programming language and its numerical mathematics extension NumPy.
Official [website](https://matplotlib.org/) |
[Wikipedia](https://en.wikipedia.org/wiki/Matplotlib)

Install Matplotlib : Open command prompt type `pip install matplotlib` press enter











