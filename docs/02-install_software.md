# Install Software

![](images/R_studio_LaTeX_header.png)
You will need to install both $R$ and $R Studio$, but $\LaTeX$ is optional.


## The R Programing Language

> The **“Comprehensive R Archive Network” (CRAN)** is a collection of sites which carry identical material, consisting of the $R$  distribution(s), the contributed extensions (packages), and documentation for $R$.  From $CRAN$, you can obtain the latest official FREE release of BASE $R$.

<div class="rmddownload">
<p>Go to: <a href="http://www.r-project.org">www.r-project.org</a></p>
<ul>
<li>Choose a CRAN mirror close to your geographical location<br />
</li>
<li>Select <strong>base</strong> <span class="math inline">\(R\)</span> for your computer <em>(Windows, Mac, ect.)</em><br />
</li>
<li>Once it is downloaded, run the instalation.<br />
</li>
<li>The defaults are good...don't change them...just keep clicking <em>'Next'</em></li>
</ul>
</div>

![](images/CRAN_download.PNG){width=600px}

![](images/CRAN_mirror.PNG){width=600px}

![](images/CRAN_version.PNG){width=600px}

![](images/CRAN_select.PNG){width=600px}


<div class="rmdlink">
<p>The <span class="math inline">\(R\)</span> Project website has an extensive <a href="https://cran.r-project.org/doc/FAQ/R-FAQ.html">FAQ</a></p>
</div>


<div class="rmdlightbulb">
<p>Each new release of <span class="math inline">\(R\)</span> is given a name that references a Peanuts strip or film. Read some of the past names and find out where they came from: <a href="https://livefreeordichotomize.com/2017/09/28/r-release-names/">blog post</a></p>
</div>

---------------------------------

## The R Studio IDE

> **RStudio** is a company that is also an active member of the $R$ community. They believe free and open source data analysis software is a foundation for innovative and important work in science, education, and industry. Their namesake software, $RStudio$, is an integrated development environment (IDE) for $R$. It includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging and workspace management. 

<div class="rmddownload">
<p>Go to: <a href="http://www.rstudio.com">www.rstudio.com</a></p>
<ul>
<li>Select the FREE Open Source <strong>Desktop</strong> Edition of <span class="math inline">\(R Studio\)</span></li>
<li>The defaults are good...don't change them...just keep clicking <em>'Next'</em></li>
</ul>
</div>

![](images/RStudio_download.PNG){width=600px}

![](images/RStudio_version.PNG){width=600px}

![](images/RStudio_platform.PNG){width=600px}


<div class="rmdlink">
<p><span class="math inline">\(R Studio\)</span> has an entire <a href="https://www.rstudio.com/online-learning/">online learning library</a>. It is full of helpful links and resources for R programing, R markdown, and statistics.</p>
</div>

<div class="rmdlightbulb">
<p><strong>Note:</strong> The <a href="https://www.r-consortium.org/"><span class="math inline">\(R Consortium\)</span></a> is a collaboration between the <span class="math inline">\(R\)</span> Foundation, <span class="math inline">\(RStudio\)</span>, <span class="math inline">\(Microsoft\)</span>, <span class="math inline">\(TIBCO\)</span>, <span class="math inline">\(Google\)</span>, <span class="math inline">\(Oracle\)</span>, <span class="math inline">\(HP\)</span> and others. It’s chartered to fund and inspire ideas that will enable <span class="math inline">\(R\)</span> to become an even better platform for science, research, and industry.</p>
</div>



---------------------------------

## TeX (optional)



> $\TeX$ or $LaTeX$ is a typesetting or formatting system that is commonly used in printing and publishing, especially anything with formulas (see https://texfaq.org/FAQ-whatTeX).  It is NOT NEEDED to run $R$, but $R Studio$ must have access to it in order to `knit` a $R Notebook$ into a `.pdf` file.  There are many versions, but the following are the ones that work best with $R$, depending on your computer's platform.


### Mac - use `MacTeX`


<div class="rmddownload">
<p>Go to: <a href="http://tug.org/mactex/" class="uri">http://tug.org/mactex/</a></p>
<ul>
<li>Download (5+ min) to a folder and them double click on the <strong>PKG file</strong></li>
<li>Follow the installation instructions.</li>
<li>You don't need to open anything after MacTeX is finished installing.</li>
</ul>
</div>


![](images/MacTeX_download.PNG){width=600px}



### Windows - use `MikTeX`

<div class="rmddownload">
<p>Go to: <a href="http://miktex.org/download" class="uri">http://miktex.org/download</a></p>
<ul>
<li>Pick the latest version of the <strong>Net Installer</strong>, not the Basic!<br />
</li>
<li>You need the full version 64-bit is better, if you have a 64-bit machine<br />
</li>
<li>When your download is complete, run the downloaded installer.<br />
</li>
<li>Windows may ask you if you want to <em>“allow this app from an unknown publisher to make changes to your PC”</em>. If it does, make sure to click <strong>Yes!</strong><br />
</li>
<li>This is the slowest part...</li>
</ul>
</div>

![](images/MikTeX_download.PNG){width=600px}


### New Option: the `tinytex` package???
 
 
`tinyteX` is still a relatively new project which strives to offer all the functionality of $\LaTeX$, but remain lightweight and easier to maintain.  As it is so new, we are not adopting it currently, but keeping an eye on what is to come.

<div class="rmdlink">
<p>Keep an eye on the developing <code>tinytex</code> package by checking back to it's <a href="https://yihui.name/tinytex/">home page</a>.</p>
</div>
