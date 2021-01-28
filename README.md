# Basic softwares installation
Lists the softwares any new member of MPG Partners might need and details the installation process.

# Direct installations
We recommend downloading the following softwares :
* ![alt text](https://github.com/Eich-Barry-mpg/Basic-softwares-installation/blob/main/Variables%20environnement%20bis.png=250x250) [R](https://www.r-project.org): use any CRAN mirror for download
* [RStudio](https://rstudio.com): see the download link, then choose the free version
* [MiKTeX](https://miktex.org): see the download tab
* [Everything](https://www.voidtools.com/downloads/)
* [GitHub Desktop](https://desktop.github.com)
* [Visual Studio Code](https://code.visualstudio.com)
* [Intel® oneAPI Math Kernel Library](https://software.intel.com/content/www/us/en/develop/articles/oneapi-standalone-components.html#onemkl) : download "Intel oneAPI Math Kernel Library for Windows" file


Those installations should be fine using the latest (64 bits) version and the default settings for each software .
In case some issues are encountered, here are the detailed versions used as of January 2021 :
* R : [4.0.3](https://cran.rstudio.com)
* RStudio: [1.4.1103](https://rstudio.com/products/rstudio/release-notes/)
* Miktex: [21.1](https://miktex.org/download)

# RMarkdown
Once R and RStudio are installed, open the latter.
In the console, enter "*install.packages("rmarkdown")*" to install [RMarkdown](https://rmarkdown.rstudio.com/index.html).

# Python

## Installation
First, download [Python 3.7.7](https://www.python.org/downloads/release/python-377/) (select *Windows x86-64 executable installer*).
Choose the customized istallation, and in the custom parameters :
* install Python "at the root" : ("*C:\Python*")
* make sure to "*add Python to the PATH*"
* make sure pip will be installed by typing: "*pip*"
* install pandas by typing: "*pip install pandas*"
* install numpy by typing: "*pip install numpy*" (might indicate that numpy is already installed)
* install matplotlib by typing: "*-m pip install -U matplotlib*"
Don't hesitate to use *Everything* to check if "pandas", "numpy" and "matplotlib" are installed (just look for their names and make sure *Everything* finds some files).

## Librairies
Open the command prompt (*invite de commande*) by typing "cmd" in the Windows search bar.
Then :
* you can check that pip is installed by typing "*pip*"

## GitHub & Codpy (in case you don't already have access to the Github files)
* Download the Github zip file (will most likely be shared by email or drive)
* Then access *Github>codpy>codpy* : you will find two "codpy" files. Copy both of them.
* Find the python directory (you can look for *python.exe* in the Everything software).
* Access *Python>Python37>Lib>site-packages*
* Paste the two copied files

![alt text](https://github.com/Eich-Barry-mpg/Basic-softwares-installation/blob/main/Transfert%20codpy.png)

## Environment variables
We now need to update the environment variables.
* In the Windows search bar, look for "*Modifier les variables d'environnement*" (typing "environment" or "variable" should suffice)
* In the new window, select "Environment variables"
Now, in the second frame ("*System variables*"), create two new variables :
* Call the first one "*PYTHONHOME*" with value "*C:\Python\Python37*"
* Call the second one "*PYTHONPATH*" with three different values (you can either separate the paths with a semicolumn, or add them separately) :
    *-"*C:\Python\Python37\DLLs*"
    *-"*C:\Python\Python37\Lib*"
    *-"*C:\Python\Python37\Lib\site-packages*"

![alt text](https://github.com/Eich-Barry-mpg/Basic-softwares-installation/blob/main/Transfert%20codpy.png)

Select the "*Path*" variable and add the value : "*C:\Python\Python37*"
![alt text](https://github.com/Eich-Barry-mpg/Basic-softwares-installation/blob/main/Transfert%20codpy.png)
Close all windows.

# Utilization
To be completed.

## Miktex
Once Miktex is installed, launch TeXworks.
Check the well-functionning of the software by copying and pasting any sample (like this [one](https://tug.org/TUGboat/sampleart.ltx)) in the console, then launching the composition button (upper-left green triangle) : another TeXworks window should open, displaying the output of the code.
