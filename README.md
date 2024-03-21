# Code Organization Guide

This guide outlines practical steps to improve the readability, maintainability, and transparency of your code for CMS data analysis projects. 

> [!NOTE]
> **Write and organize your code as if a stranger will be reading and running it.** The following should help you explicitly state the implied logic of your code so that it can be understood and updated for future use. 


## Contents 
* Writing Clean & Modular Code
* Storage and Version Control
* Publishing Code on GitHub





## Writing Clean & Modular Code

**Start your file with a header** to to document author, description, input files, and output files. 

**Try commenting first.** You may benefit from outlining your logic in comments *before* you write your code. This will help you think through your process, which will should help you avoid mistakes and save time in the long run. 

**Write a comment for every 1-4 lines of code, focusing on quality over quantity.** While too much is probably better than too little, excessive comments can make your code difficult to read. 

**Avoid redundant comments.** Good code should be clear enough to explain what it is doing, so comments should instead explain what is *not* apparent from the code. 

**Comment the *why* of your code rather than the *what*.** This might include: 

* What the values of your constructed variable mean 
* Why you need to construct a variable 
* Why you made an unexpected choice (e.g. formatting quirks of a certain state Medicaid file)
* Bugs you ran into along the way

See this guide on [best practices for writing code comments](https://stackoverflow.blog/2021/12/23/best-practices-for-writing-code-comments/). 

**Follow consistent naming conventions** for your variables, dataframes/datasets, functions/macros, etc.
Clear, specific, and consistent naming will reduce the need to explain what variables are in the code. 

See the following guides for mode detail on formatting and naming conventions. 

* [Python - PEP 8 Style Guide](https://peps.python.org/pep-0008/)
* [SAS - Programming Guidelines](https://support.sas.com/resources/papers/proceedings/proceedings/sugi31/123-31.pdf)

**Modular code breaks walls of code into smaller building blocks that perform discrete tasks.** These building blocks are easier to read, test, update, and combine with each other. 

**Refactor your code**: From time to time, go back and restructure your code to improve its readability, maintainability, or performance. Try the following: 

* break your script into functions 
* reduce the number of dependencies 
* remove duplication
	* e.g. combine two similar scripts for processing TAF IP and TAF OT files into one function for processing either file. 




## Storage and Version Control


Create a repository on the Konetzka Lab group on the Research Computing Group GitLab server for internal version control. 

> [!WARNING]
> Users of cms-share must do their internal version control on the RCG GitLab servers to protect CMS data from accidentally being published in code. 


Store each project under your user folder within your DUA folder in cms-share. **Remember that if you are working under multiple data use agreements, you must store your scripts, analytical datasets, and output in the correct DUA folder.** 

Within each project folder, create separate folders for code, data, and output. 

  
## Publishing Code

**Before sending out your paper, do an internal code review to make sure your results are valid.** Provide your GitLab repository to a teammate on your DUA and see if they 1) agree with your logic and 2) can understand your code well enough to rerun your analysis. 

> [!WARNING]
> Double check that there aren't any results in your code to avoid violating the [CMS cell suppression policy](https://resdac.org/articles/cms-cell-size-suppression-policy). 

**Publish completed code at github.com/konetzka-lab under a new repository.** 

**Always create a README.md file for your repository.** This file should be detailed enough for someone else to run your code. Include the following information: 

* General description 
* Software used
* Write a description of each step of your analysis, including a table with the following details for each file: 
	* file name 
	* input data 
	* output data
	* constructed variables 

You can find a great example of a readme file [here](https://github.com/sanghavi-lab/nhc_falls). 
