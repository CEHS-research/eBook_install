--- 
title: "Encyclopedia of Quantitative Methods in R, vol. 0: Setting up Your Computer"
author: "Sarah Schwartz & Tyson Barrett"
date: "Last updated: 2018-08-15"
documentclass: book
description: "Getting started with R and R Studio: installing software and package management."
knit: "bookdown::render_book"
cover-image: "EQM_v0_cover.png"
github-repo: cehs-research/eBook_install
site: bookdown::bookdown_site
output:
  bookdown::gitbook:
    split_bib: false
bibliography: [book.bib, packages.bib]
biblio-style: "apalike"
link-citations: yes
---



# Welcome {-}

![](images/EQM_img/EQM_v0_header.png)









## Preface {-}

This encyclopedia of eBooks is being developed by the [Office of Research Services](https://cehs.usu.edu/research/index) to serves the faculty and graduate students in the [College of Education and Human Services](https://cehs.usu.edu/) at [Utah State University](http://www.usu.edu/).  



The three main purposes are to: 

* Provide reference material for graduate quantitative methods courses *(EDUC/PSY 6600, EDUC/PSY 7610, PSY 7650, ect.)*  
* Support college wide workshops given by the [Statistical Consulting Studio](https://cehs.usu.edu/research/statstudio/index) and [Data Science and Discover Unit](https://cehs.usu.edu/research/dsdu/index)
* Facilitate individual consultations with the authors pertaining to research.



This massive undertaking started during the summer of 2018 and is far from complete.  The outline of seven volumes is given below despite any one being complete.  Feedback is welcome via either author's email.


<table>
 <thead>
  <tr>
   <th style="text-align:left;"> Volumne </th>
   <th style="text-align:left;"> Link </th>
   <th style="text-align:left;"> Content </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v0_button.png){width=150px} </td>
   <td style="text-align:left;"> [Vol. 0](https://cehs-research.github.io/eBook_install/) </td>
   <td style="text-align:left;"> **Setting up Your Computer:** Installing R, R Studio, and Packages </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v1_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 1 </td>
   <td style="text-align:left;"> **Data Management:** Importing, Sub-Setting, Creating Variables, and Saving </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v2_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 2 </td>
   <td style="text-align:left;"> **Exploratory Data Analysis:** Summary Statistics and Descriptive Visualizations </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v3_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 3 </td>
   <td style="text-align:left;"> **Testing Mean Differences:** t-tests, ANOVA, RM ANOVA, and post hoc tests </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v4_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 4 </td>
   <td style="text-align:left;"> **Multiple Linear Regression:** Correlation, Model Fit, Generalize, and Plot </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v5_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 5 </td>
   <td style="text-align:left;"> **Multilevel Models (RM Regression):** ICCs, MLM/HLM, and GEEs </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v6_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 6 </td>
   <td style="text-align:left;"> **Structural Equation Modeling:** EFA, CFA, Path Analysis, and SEM </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ![](images/EQM_img/EQM_v7_button.png){width=150px} </td>
   <td style="text-align:left;"> Vol. 7 </td>
   <td style="text-align:left;"> **Additional Topics:** Room for Future Expansio </td>
  </tr>
</tbody>
</table>






## Authors {-}


| [Dr. Sarah Schwartz](http://www.sarahschwartzstats.com/) | [Dr. Tyson Barrett](http://tysonbarrett.com/) |
|:----:|:----:|
| ![](images/Sarah_headshot.jpg){width=300px} | ![](images/Tyson_headshot.jpg){width=300px} |
| Sarah.Schwartz@usu.edu | Tyson.Battett@usu.edu |
| [Statistical Consulting Studio](https://cehs.usu.edu/research/statstudio/index)  | [Data Science and Discover Unit](https://cehs.usu.edu/research/dsdu/index) |
| ![](images/StatStudioLogo_dark_small.png){width=300px}  |![](images/dsdu_logo.PNG){width=300px} |







## Why R ?  {-}



<div class="rmdconstruct">
<p><strong>ADD SECTION:</strong> R vs. SPSS, SAS, Stata, ect...</p>
</div>




[No more excuses: R is better than SPSS for psychology undergrads, and students agree](https://datahowler.wordpress.com/2016/09/10/no-more-excuses-r-is-better-than-spss-for-psychology-undergrads-and-students-agree/)




## FYI  {-}

The entire encyclopedia is written in $R Markdown$, using $R Studio$ as the text editor and the `bookdown` package to turn a collection of markdown documents into a coherent whole. The book's source code is hosted on GitHub, at https://github.com/cehs-research/eBook_install. If you notice typos or other issues, feel free to open an issue on GitHub or send me a pull request. If you do the latter, in your commit message, please add the sentence "I assign the copyright of this contribution to Dr.s Schwartz and Barrett," so that I can maintain the option of publishing this book in other forms.

This work is licensed under the [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode) License. 



![](images/Education_Logo_WHITE-02.png){width=250px}
