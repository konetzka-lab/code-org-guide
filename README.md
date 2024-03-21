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

**Avoid writing comments that just restates what the code is doing.** Good code should be self-explanatory in that regard, so comments should instead explain what is *not* apparent from the code. 

**Comment the *why* of your code rather than the *what*.** This might include: 

* What the values of your constructed variable mean 
* Why you need to construct a variable 
* Why you made an unexpected choice (e.g. formatting quirks of a certain state Medicaid file)
* Bugs you ran into along the way 


## Cataloging Code

Store each project under your user folder within your DUA folder in cms-share. **Remember that if you are working under multiple data use agreements, you must store your scripts, analytical datasets, and output in the correct DUA folder.** 

Within each project folder, create folders for code, data, and output. For example: 


  


## Publishing Code

Publish completed code at github.com/konetzka-lab under a new repository. 

### Creating a repository
### Creating a README.md for your repository 
