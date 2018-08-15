--- 
title: "Encyclopedia of Quantitative Methods in R, vol. 0: Setting up Your Computer"
author: "Sarah Schwartz & Tyson Barrett"
date: "Last updated: 2018-08-14"
site: bookdown::bookdown_site
output:
  bookdown::gitbook:
    split_bib: false
documentclass: book
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
github-repo: cehs-research/eBook_install
description: "Getting started with R and R Studio: installing software and package management."
url: https://github.com/CEHS-research/eBook_install
cover-image: "EQM_v0_cover.png"
---



# Welcome {-}

![](images/EQM_img/EQM_v0_header.png)



## Preface {-}

This encyclopedia of eBooks is being developed by [Sarah Schwartz](http://www.sarahschwartzstats.com/) and [Tyson Barrett](http://tysonbarrett.com/), of the [Office of Research Services](https://cehs.usu.edu/research/index), to support faculty and graduate students in the [College of Education and Human Services](https://cehs.usu.edu/) at [Utah State University](http://www.usu.edu/).  It serves as reference material for graduate courses (EDUC/PSY 6600, EDUC/PSY 7610, PSY 7650, ect.), as well as college wide workshops and individualized consultation from the [Statistical Consulting Studio](https://cehs.usu.edu/research/statstudio/index) and the [Data Science and Discover Unit](https://cehs.usu.edu/research/dsdu/index).


![](images/cehs_statstudio_dsdu.PNG)


-------------

## Background FAQs {-}



### What is R ? {-}

> $R$ is a language and environment for statistical computing and graphics. [@R-base]

$R$ provides a wide variety of **statistical** *(linear and nonlinear modelling, classical statistical tests, time-series analysis, classification, clustering, ...)* and **graphical** techniques, and is highly extensible. The $S$ language is often the vehicle of choice for research in statistical methodology, and $R$ provides an Open Source route to participation in that activity.

One of $R$’s strengths is the ease with which well-designed publication-quality plots can be produced, including mathematical symbols and formulae where needed. Great care has been taken over the defaults for the minor design choices in graphics, but the user retains full control.

-------------------------

### What is R Markdown ? {-}

According to [R Studio](www.rstudio.com):

> "R Markdown is a format that enables easy authoring of reproducible web reports from R. It combines the core syntax of Markdown (an easy-to-write *plain text* format for web content) with embedded *$R$ code chunks* that are run so their output can be included in the final document".



-------------------------------

### What is Dynamic Reporting? {-}

From [Penn State Statistics](https://onlinecourses.science.psu.edu/statprogram/markdown): 

The traditional way to write a report:

1. Run your analysis in software, like SPSS or R and manually save our output
    * *i.e. saving the ANOVA table or using `pdf()` to save the graphs*  


2. Type your your description and interpretation in a text editor like *Word*
    * *either drag/drop tables and figures, or worse copy-paste and retype all the numbers*


A report written in this way can be problematic.  For instance, imagine your *Mentor/collaborator/journal reviewer*  telling you that they want to use a sub-sample instead of the entire sample. Or to include a nother variable.  You would have to redo all of your work!! 

Therefore, in this way **dynamic also means reproducible**, in the sense that people who get the file from you can reproduce the entire work in the report.


-------------------

### How does R Markdown work out to be a `.pdf` or `.html` file? {-}

$R Markdown$ is a file with the file extension `.Rmd`, the `knitr` package will then transform the file into a *Markdown* file with the extension `.md.` Then $R Studio$ can [@xie2015]:

  * Use $LaTeX$ to transform the file into a `.pdf` 
    
  * Load another package called $markdown$ to transform the file into `.html`   
    
  * Use Pandoc to even convert to file to a `Word` document (ugly)

![](images/processRStudio.png)


The professionals ar $R Studio$ show it better at their [website](https://rmarkdown.rstudio.com/index.html).

----------------------

### Is this a popular method for creating reports? {-}

Check out [Rpubs](http://rpubs.com/). This website shares lots of documents written in the way we will introduce below.




<!--chapter:end:index.Rmd-->

# An Overview

![](images/headers/R_studio_LaTeX_header.png)


Before we get busy downloading and installing the actual software, here is the big picture.

-------------------------------

## R vs. R Studio

First time users often confuse by all the different uses of the letter "R". 

| $R$ | $R Studio$ |
| ---|-----------|
| Engine | Dashboard |
| Install and Ignore | Interact with Constantly | 
| ![](images/car_engine.jpg){width=500px} | ![](images/car_dashboard.jpg){width=500px} |


> More precisely, $R$ is a *programming language* that runs computations while $R Studio$ is an *integrated development environment (IDE)* that provides an interface by adding many convenient features and tools. So the way of having access to a speedometer, rearview mirrors, and a navigation system makes driving much easier, using $RStudio’s$ interface makes using $R$ much easier as well.  - [Chester Ismay and Albert Y. Kim](https://ismayc.github.io/moderndive/index.html)

For a more in-depth discussion on the difference between $R$ and $R Studio$ IDE, watch this [DataCamp video (2m52s)](https://campus.datacamp.com/courses/working-with-the-rstudio-ide-part-1/orientation?ex=1).




-------------------------------

## R Markdown vs. R Notebook





-------------------------------

## The Magic of Knit'ing



![](images/hex/rmarkdown-200x232.png)

 
> $R Markdown$ documents are fully reproducible. Use a productive **notebook** interface to weave together narrative text and code to produce elegantly formatted output. Use multiple languages including $R$, $Python$, and $SQL$ [@R-rmarkdown].


![](images/hex/knitr-200x232.png)


> `knitr` is an engine for dynamic report generation with $R$. It is a package in the statistical programming language $R$ that enables integration of **R code** into $LaTeX$, $LyX$, $HTML$, $Markdown$, $AsciiDoc$, and $text$s documents [@R-knitr].


----------------

\begin{rmdtip}
\emph{Helpful Website:}
\href{https://www.statmethods.net/stats/index.html}{Quick R: Basic
Statistics}
\end{rmdtip}



<!--chapter:end:01-Overview.Rmd-->

# Install R

![](images/Rlogo_200.png)

Here is where we talk about installing R.

-----------

## First Time Installation

> Go to: [www.r-project.org](http://www.r-project.org) 

Get the latest released version of FREE **Base** $R$ from $CRAN$ 

* Choose a mirror close to your geographical location
* Select **base** $R$ for your computer *(Windows, Mac, ect.)*
* The defaults are good...don't change them...just keep clicking *'Next'*

-----------

## Update Regularly




<!--chapter:end:02-install_R.Rmd-->

# Install R Studio

![](images/rstudiosticker.png)

Here is where we talk about installing R Studio.

-----------

## First Time Installation

> Go to: [www.rstudio.com](http://www.rstudio.com) 

Get the latest version of the FREE Open Source **Desktop** Edition of R Studio

* The defaults are good...don't change them...just keep clicking *'Next'*

-----------

## Update Regularly


-----------

## Panel Layout

<!--chapter:end:03-install_Rstudio.Rmd-->

# Install TeX

![](images/latex.png)


Here is where we talk about installing Tex.

-----------

## Use `tinytex` package


-----------

## Mac - use `MacTeX`

> Go to: [http://tug.org/mactex/](http://tug.org/mactex/) 

* Download (5+ min) to a folder and them double click on the **PKG file**
* Follow the installation instructions.
* You don't need to open anything after MacTeX is finished installing. 

-----------

## Windows - use `MikTeX`

> Go to: [http://miktex.org/download](http://miktex.org/download)

* Pick the latest version of the **Net Installer**, not the Basic! 
* You need the full version 64-bit is better, if you have a 64-bit machine
* When your download is complete, run the downloaded installer. 
* Windows may ask you if you want to *“allow this app from an unknown publisher to make changes to your PC”*. If it does, make sure to click **Yes!**
* This is the slowest part...

<!--chapter:end:04-install_tex.Rmd-->

# Install Packages

We describe packages and their management

-----------

## What are packages

> **R packages** are collections of functions and data sets developed by the community. They increase the power of **R** by improving existing base **R** functionalities, or by adding new ones.

More information may be found here:  https://www.datacamp.com/community/tutorials/r-packages-guide 


-----------

## Installing packages (via the user interface)

> You only need to INSTALL packages ONCE per computer.


In **R Stuido**:

1. Click on the **Packages** tab the panel with the most tabs
2. Click on the word **Instsall** just under and to the left of the tab
2. In the **Packages** box, type in the name of the packages you would like to download.  You can do several at once, just seperate them with multiple spaces or a comma.

*Note: Leave the installation library path as the default.  Also, make sure the box for 'Installing dependencies' is checked.*

![](images/Install_Package_Screenshot.png)


You can *copy-and-paste* the following list into the box (labeled 3) to load the packages that we use most commonly all at once. 

> tidyverse, furniture, pander, stargazer, texreg, xtable, RColorBrewer, gghighlight, ggthemes, ggfortify, ggalt, ggExtra, GGally, ggeffects, corrplot, gpairs, gridextra, likert, vcd, scales, cowplot, yarrr, psych, polycor, corpcor, sjlabelled, sjPlot, sjmisc, sjstats, Hmisc, labelled, afex, emmeans, corpcor, multicomp, multcompView, car, effects, predictmean, nlme, lme4, lmerTest, HLMdiag, geepack, gee, gee4, optimx, MuMIn, lavaan, OpenMx, sem, semPlot, randomForest, randomForestSRC, ggRandomForests, party, partykit, mgcv, glmnet, survival, caret, bookdown, blogdown, tidytex, xaringan, REDCapR, redcapAPI, devtools, testthat, roxygen2

When you click the **Install** buttom, a smaller window may asks if you would like to re-start $R$ prior to installing, choose "no" and manually close and open the $R Studio$ program once all packages have been downloaded, unpacked, and checked.  This may take a few minutes, especially if you have selected multiple packages.  


> See Chapter 6 for more information on how to install packages another way (via syntax code), as well as website links for each package.




-----------

## Updating packages





<!--chapter:end:05-install_packages.Rmd-->

# Kniting Notebooks

------------

## Storing all associated files 

If you are using any files, such as *datasets* or *images*, they need to be stored in the same folder location as the R Notebook (`.Rmd` file).

This folder location must be the **Working Directory** for the R Studio session.  If you opened your `.Rmd` notebook file by double-clicking on its name, then this should be the case.  


------------

## Setting the working directory

To ensure that R Studio knows where to find the files, you can manually set the **Working Directory** through the menu:

* Click `Session`
* Select `Set Working Directory` by hovering your mouse over it
* Click on `To Source File Location`

![](images/Set_wd_source.png)

You can double check that you were successful by 

* Click on the `Files` tab in the many-tab panel
* Click on the button with the gear that says `More`
* Click `Go To Working Directory`

At this point you should see all the files that reside in the folder location where the open `.Rmd` files is also saved. 

![](images/files_goto_wd.png)

------------

## Press the Knit button

<!--chapter:end:08-steps.Rmd-->





<!--chapter:end:99-refs.Rmd-->

