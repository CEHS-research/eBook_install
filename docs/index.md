--- 
title: "Encyclopedia of Quantitative Methods in R, vol. 0: Setting up Your Computer"
author: "Sarah Schwartz & Tyson Barrett"
date: "Last updated: 2018-08-16"
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


<table>
 <thead>
  <tr>
   <th style="text-align:center;"> Volume </th>
   <th style="text-align:left;"> Title </th>
   <th style="text-align:left;"> Content </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> 0. Software </td>
   <td style="text-align:left;"> [Setting up Your Computer](https://cehs-research.github.io/eBook_install/) </td>
   <td style="text-align:left;"> Installing R, R Studio, and Packages </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 1. Wrangling </td>
   <td style="text-align:left;"> Data Management </td>
   <td style="text-align:left;"> Importing, Sub-Setting, Creating Variables, and Saving </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 2. Exploratory </td>
   <td style="text-align:left;"> Exploratory Data Analysis </td>
   <td style="text-align:left;"> Summary Statistics and Descriptive Visualizations </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 3. ANOVA </td>
   <td style="text-align:left;"> Testing Mean Differences </td>
   <td style="text-align:left;"> t-tests, ANOVA, RM ANOVA, and post hoc tests </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 4. Regression </td>
   <td style="text-align:left;"> Regression </td>
   <td style="text-align:left;"> Correlation, Model Fit, Generalize, and Plot </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 5. Multilevel </td>
   <td style="text-align:left;"> Multilevel Models </td>
   <td style="text-align:left;"> Clustered and Longitudinal - ICCs, MLM/HLM, and GEEs </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 6. SEM </td>
   <td style="text-align:left;"> Structural Equation Modeling </td>
   <td style="text-align:left;"> EFA, CFA, Path Analysis, and SEM </td>
  </tr>
  <tr>
   <td style="text-align:center;"> 7. Other </td>
   <td style="text-align:left;"> Additional Topics </td>
   <td style="text-align:left;"> Room for Future Expansion </td>
  </tr>
</tbody>
</table>


<div class="rmdconstruct">
<p><strong>This eBook is under construction: check back often.</strong> This massive undertaking started during the summer of 2018 and is far from complete. The outline of seven volumes is given above despite any one being complete. Feedback is welcome via either author's email.</p>
</div>


## Authors {-}


<table>
 <thead>
  <tr>
   <th style="text-align:center;font-size: 20px;"> Dr. Sarah Schwartz </th>
   <th style="text-align:center;font-size: 20px;"> Dr. Tyson Barrett </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> ![](images/Sarah_headshot.jpg){width=300px} </td>
   <td style="text-align:center;"> ![](images/Tyson_headshot.jpg){width=300px} </td>
  </tr>
  <tr>
   <td style="text-align:center;"> [www.SarahSchwartzStats.com](http://www.sarahschwartzstats.com/) </td>
   <td style="text-align:center;"> [www.TysonBarrett.com](http://tysonbarrett.com/) </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Sarah.Schwartz@usu.edu </td>
   <td style="text-align:center;"> Tyson.Battett@usu.edu </td>
  </tr>
  <tr>
   <td style="text-align:center;"> [Statistical Consulting Studio](https://cehs.usu.edu/research/statstudio/index) </td>
   <td style="text-align:center;"> [Data Science and Discover Unit](https://cehs.usu.edu/research/dsdu/index) </td>
  </tr>
  <tr>
   <td style="text-align:center;"> ![](images/StatStudioLogo_dark_small.png){width=300px} </td>
   <td style="text-align:center;"> ![](images/dsdu_logo.PNG){width=300px} </td>
  </tr>
</tbody>
</table>






## Why R ?  {-}



<div class="rmdconstruct">
<p><strong>ADD SECTION:</strong> R vs. SPSS, SAS, Stata, ect...</p>
<p>FREE, accessable, not any harder than others to learn reproducibity</p>
</div>


<div class="rmdlink">
<p><strong>Check it out:</strong> an article from Fall 2016... <a href="https://datahowler.wordpress.com/2016/09/10/no-more-excuses-r-is-better-than-spss-for-psychology-undergrads-and-students-agree/">No more excuses: R is better than SPSS for psychology undergrads, and students agree</a></p>
</div>




## FYI  {-}

The entire encyclopedia is written in $R Markdown$, using $R Studio$ as the text editor and the `bookdown` package to turn a collection of markdown documents into a coherent whole. The book's source code is hosted on GitHub, at https://github.com/cehs-research/eBook_install. If you notice typos or other issues, feel free to open an issue on GitHub or send me a pull request. If you do the latter, in your commit message, please add the sentence "I assign the copyright of this contribution to Dr.s Schwartz and Barrett," so that I can maintain the option of publishing this book in other forms.

This work is licensed under the [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode) License. 



![](images/Education_Logo_WHITE-02.png){width=250px}
