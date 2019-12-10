Created: 12/4/2019  
DATA 512 Human Centered Data Science  
Peter Meleney  

# An Introduction to Statistical Learning: Applications in Python

## Introduction

### Objective
The objective of these notebooks is to give aspiring data scientists, who are familiar with python 3.x, but not R, access to the laboratory sections of the book "An introduction to Statistical Learning with Applications in R" (ISLR).  This repository is meant to be an complement to and extention of JWarmhoven's excellent repository availabale here: https://github.com/JWarmenhoven/ISLR-python/.

### Motivation
It is my opinion that ISLR is an excellent introduction to data science, and I have read it many times.  However I have always been frustrated that it was written exclusively using the R language for examples and labs.  In my research for this project I found that R was the predominate language of data science professionals when the book was written in 2013 (see figure 1), however that changed rapidly between 2013 and today (2019) when python is the most prevelant language among data science professionals (see figure 2).  

![image of data science prefs 2013](https://github.com/pmeleney/data512_project/images/data_science_prefs_2013.PNG)

In 2013, R was the dominate language among data science professionals.  In this study conducted by KD Nuggets, which asked the question: "What programming/statistices languages you used for an analytics / data mining / data science work in 2013?," among the 713 respondents to that question, over 60% of them used R, and only 38.8% of them used python.  

![image of data science prefs 2018](https://github.com/pmeleney/data512_project/images/data_science_prefs_2018.PNG)

However by 2018, a much larger study conducted by Kaggle which asked "What specific programming language do you use most often?" among the 23,859 respondents 54% responded that Python was the language they used most, followed by R at only 13%.  This may explain why the authors originally chose R as the consensus language among data professionals in 2013, but the evolution of the field towards use of python strongly motivates my work in its translation to Python.

### Justifications

#### Jupyter Notebook
Jupyter Notebooks provide an excellent platform for creating the literate, interactive programming documents that I wish to create for this project.  Many data science professionals as familiar with jupyter notebooks, and I am fluent in their use, making them an excellent choice for this project.

#### Python 3.7
Though Python 3.8.0 was officially released on October 14, 2019, it is not yet supported by Anaconda, which is the distribution of Python I use to manage environments.  I do not expect that any lack of the expansions in the lexecon of Python will inhibit our exploration of these introductory ideas. 

#### Scikit-Learn
Whenever possible we will use the scikit-learn version of machine learning models.  Scikit-learn is an excellent data science module available as a free, opensource, and commercially usable set of tools for python.  It is what I originally learned on and I think that any aspiring data scientist should be introduced to its wonderful set of tools.  We will be using the latest version of scikit-learn, version 0.22 - more information is available here: https://scikit-learn.org/stable/.

#### Scripting Coding Style
There are several stylistic options to choose from when writing python code.  In heigherarctical order there is scripting style, functional style, and object-oriented style.  For this project I will use the scripting style of programming because it is most condusive to working in jupyter notebooks - e.g. functions don't need to be speficied and then run, the script can be run directly in the interactive layer.  I anticipate using functions sparsely throughout the project, mostly to facilitate data munging.

## Data
Detailed data exploration will be left to the individual chapters, as extensive exploration here would be too long, and lead to the reader flipping back and forth between this README document and the jupyter notebook.  Here I will note that all the data, with the exception of the "Boston" data set, has been released by the authors of ISLR under the GPL-2 license for reuse (https://cran.r-project.org/web/packages/ISLR/index.html).  .  The “Boston” dataset is used widely as a benchmark throughout data science and computer science, and is made available through the University of Toronto Computer Science Department at https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html.  The data was originally collected by the U.S. Census Service, and so is in the public domain.

|**Name**|**Description**|
|--------|:---------------------|
|Boston|	Housing values and other information about Boston suburbs.|
|Hitters|	Records and salaries for baseball players.|
|Smarket|	Daily percentage returns for S&P 500 over a 5-year period.|
