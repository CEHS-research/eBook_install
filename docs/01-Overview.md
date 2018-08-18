# Overview




![](images/headers/manyRs.png)


Before we get busy downloading and installing the actual software, here is the big picture.

----------------------

## R vs. R Studio

<table>
 <thead>
  <tr>
   <th style="text-align:center;"> R </th>
   <th style="text-align:center;"> R Studio </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> ![](images/Rlogo_200.png){width=100px} </td>
   <td style="text-align:center;"> ![](images/rstudiosticker.png){width=200px} </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Programing Language </td>
   <td style="text-align:center;"> Interface Program </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Install and Ignore </td>
   <td style="text-align:center;"> Interact with Constantly </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Engine </td>
   <td style="text-align:center;"> Dashboard </td>
  </tr>
  <tr>
   <td style="text-align:center;"> ![](images/car_engine.jpg){width=500px} </td>
   <td style="text-align:center;"> ![](images/car_dashboard.jpg){width=500px} </td>
  </tr>
</tbody>
</table>


> Many users think of $R$ as a statistics system. We prefer to think of it of an environment within which statistical techniques are implemented. $R$ can be extended (easily) via packages. There are about eight packages supplied with the $R$ distribution and many more (over 10,000) are available through the $CRAN$ family of Internet sites covering a very wide range of modern statistics.
>
> [www.r-project.org](https://www.r-project.org/about.html)


Where as $R$ is a *programming language* that runs computations, $R Studio$ is an *integrated development environment (IDE)* that provides an interface by adding many convenient features and tools. So the way of having access to a speedometer, rearview mirrors, and a navigation system makes driving much easier, using **$RStudio’s$ interface makes using $R$ much easier** as well.  - [Chester Ismay and Albert Y. Kim](https://ismayc.github.io/moderndive/index.html)




<div class="rmdlink">
<p>For a more in-depth discussion on the difference between <span class="math inline">\(R\)</span> and <span class="math inline">\(R Studio\)</span> IDE, watch this <a href="https://campus.datacamp.com/courses/working-with-the-rstudio-ide-part-1/orientation?ex=1">DataCamp video (2m52s)</a>.</p>
</div>

----------------------

## R Markdown vs. R Notebook

<table>
 <thead>
  <tr>
   <th style="text-align:center;"> R Markdown </th>
   <th style="text-align:center;"> R Notebook </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> ![](images/hex/rmarkdown-200x232.png) </td>
   <td style="text-align:center;"> ![](images/Rnotebook.png){width=225px} </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Plain text that includes shorthand notation to denote formatting, instead of relying on a text editor program display (MS Word).  Files are saved with the `.Rmd` extension. </td>
   <td style="text-align:center;"> A specific kind of `.Rmd` file in which the code chunks may be interactively executed/run onscreen and the results/output are shown directly below each code chunk. </td>
  </tr>
</tbody>
</table>

 
$R Markdown$ documents are fully reproducible. Use a productive **notebook** interface to **weave together narrative text and code** to produce elegantly formatted output. Use multiple languages including $R$, $Python$, and $SQL$ [@R-rmarkdown].



<div class="rmdlink">
<p><strong>More details at the R Studio website:</strong> <a href="https://rmarkdown.rstudio.com/lesson-1.html">R Markdown, lesson 1</a> and <a href="https://rmarkdown.rstudio.com/r_notebooks">R Notebooks</a></p>
</div>


----------------------

## knit-R

![](images/cartoon_knit.PNG)

With the click of a button, the `knitr` package will convert a $R notebook$ (`.Rmd`) to an intermediary *Markdown* file with the extension `.md`, which $R Studio$ will further transform to various final file types, including [@xie2015]: 

* `.pdf` using $LaTeX$ *(beautiful)*

* `.html` using another package called $markdown$ *(highly viewable)*   

* `Word` document using Pandoc *(probably be ugly)*


![](images/knitr_formats.PNG){width=500px}


`knitr` is an engine for dynamic report generation with $R$. It is a package in the statistical programming language $R$ that enables integration of **R code** into $LaTeX$, $LyX$, $HTML$, $Markdown$, $AsciiDoc$, and $text$s documents [@R-knitr].


<div class="rmdlink">
<p>The professionals ar <span class="math inline">\(R Studio\)</span> show it better at their <a href="https://rmarkdown.rstudio.com/index.html">website</a>.</p>
</div>


-------------

## More Indepth FAQs 


<div class="rmdlink">
<p><strong>Helpful Websites:</strong> <a href="https://www.statmethods.net/stats/index.html">Quick R: Basic Statistics</a> and <a href="https://libguides.library.kent.edu/statconsulting/r">Introduction to R</a></p>
</div>



### What is R ? {-}

> $R$ is a language and environment for statistical computing and graphics. [@R-base]

$R$ provides a wide variety of **statistical** *(linear and nonlinear modelling, classical statistical tests, time-series analysis, classification, clustering, ...)* and **graphical** techniques, and is highly extensible. The $S$ language is often the vehicle of choice for research in statistical methodology, and $R$ provides an Open Source route to participation in that activity.

One of $R$’s strengths is the ease with which well-designed publication-quality plots can be produced, including mathematical symbols and formulae where needed. Great care has been taken over the defaults for the minor design choices in graphics, but the user retains full control.



### What is R Markdown ? {-}

According to [R Studio](www.rstudio.com):

> "R Markdown is a format that enables easy authoring of reproducible web reports from R. It combines the core syntax of Markdown (an easy-to-write *plain text* format for web content) with embedded *$R$ code chunks* that are run so their output can be included in the final document".





### What is Dynamic Reporting? {-}

From [Penn State Statistics](https://onlinecourses.science.psu.edu/statprogram/markdown): 

The traditional way to write a report:

1. Run your analysis in software, like SPSS or R and manually save our output
    * *i.e. saving the ANOVA table or using `pdf()` to save the graphs*  


2. Type your your description and interpretation in a text editor like *Word*
    * *either drag/drop tables and figures, or worse copy-paste and retype all the numbers*


A report written in this way can be problematic.  For instance, imagine your *Mentor/collaborator/journal reviewer*  telling you that they want to use a sub-sample instead of the entire sample. Or to include a nother variable.  You would have to redo all of your work!! 

Therefore, in this way **dynamic also means reproducible**, in the sense that people who get the file from you can reproduce the entire work in the report.






### Is this a popular method for creating reports? {-}

YES!

<div class="rmdlink">
<p>Check out <a href="http://rpubs.com/">Rpubs</a>. This website shares lots of documents written in the way we will introduce below.</p>
</div>





