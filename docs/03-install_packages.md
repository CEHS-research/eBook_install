# Install Packages


![](images/headers/library.png)

We describe packages and their management

-----------

## What are packages

**R packages** are collections of functions and data sets developed by the community. They increase the power of **R** by improving existing base **R** functionalities, or by adding new ones.

<div class="rmdlink">
<p>More information may be found here: <a href="https://www.datacamp.com/community/tutorials/r-packages-guide" class="uri">https://www.datacamp.com/community/tutorials/r-packages-guide</a></p>
</div>


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

> tidyverse, furniture, pander, stargazer, texreg, xtable, kableExtra, RColorBrewer, gghighlight, ggthemes, ggfortify, ggalt, ggExtra, GGally, ggeffects, corrplot, gpairs, gridextra, likert, vcd, scales, cowplot, yarrr, psych, polycor, corpcor, sjlabelled, sjPlot, sjmisc, sjstats, Hmisc, labelled, afex, emmeans, corpcor, multicomp, multcompView, car, effects, predictmean, nlme, lme4, lmerTest, HLMdiag, geepack, gee, gee4, optimx, MuMIn, lavaan, OpenMx, sem, semPlot, randomForest, randomForestSRC, ggRandomForests, party, partykit, mgcv, glmnet, survival, caret, bookdown, blogdown, tidytex, xaringan, REDCapR, redcapAPI, devtools, testthat, roxygen2

When you click the **Install** buttom, a smaller window may asks if you would like to re-start $R$ prior to installing, choose "no" and manually close and open the $R Studio$ program once all packages have been downloaded, unpacked, and checked.  This may take a few minutes, especially if you have selected multiple packages.  


## Useful Packages



<div class="rmdlink">
<p>A curated list of awesome <span class="math inline">\(R\)</span> packages and tools: <a href="https://awesome-r.com/" class="uri">https://awesome-r.com/</a></p>
</div>


### The Tidy-Universe from $R Studio$


```r
install.packages("tidyverse")
```


> The `tidyverse` [(www.tidyverse.org)](https://www.tidyverse.org/) is an opinionated **collection of $R$ packages** designed for data science. All packages share an underlying design philosophy, grammar, and data structures. 

#### Core

The core tidyverse includes the packages that you are likely to use in everyday data analyses. As of `tidyverse 1.2.0`, the following packages are included in the core tidyverse:



```r
library(tidyverse)
```

```
## -- Attaching packages --------------------------------------------------------------- tidyverse 1.2.1 --
```

```
## v ggplot2 3.0.0     v purrr   0.2.5
## v tibble  1.4.2     v dplyr   0.7.6
## v tidyr   0.8.1     v stringr 1.3.1
## v readr   1.1.1     v forcats 0.3.0
```

```
## -- Conflicts ------------------------------------------------------------------ tidyverse_conflicts() --
## x dplyr::filter() masks stats::filter()
## x dplyr::lag()    masks stats::lag()
```

| website   | description |   
|----------:|:------------|   
| [`dplyr`](https://dplyr.tidyverse.org/)     | A Grammar of Data Manipulation |
| [`forcats`](https://forcats.tidyverse.org/) | Tools for Working with Categorical Variables *(Factors)* |
| [`ggplot2`](https://ggplot2.tidyverse.org/) | Create Elegant Data Visualisations Using the Grammar of Graphics |
| [`purrr`](https://purrr.tidyverse.org/)     | Functional Programming Tools |
| [`readr`](https://readr.tidyverse.org/)     | Read Rectangular Text Data |
| [`stringr`](https://stringr.tidyverse.org/) | Simple, Consistent Wrappers for Common String Operations *(Text)* |
| [`tibble`](https://tibble.tidyverse.org/)   | Simple Data Frames |
| [`tidyr`](https://tidyr.tidyverse.org/)     | Easily Tidy Data with `spread()` and `gather()` Functions |
   
#### Supplemental 

The tidyverse also includes many other packages with more specialised usage. They are not loaded automatically with `library(tidyverse)`, so you'll need to load each one with its own call to `library()`.



```r
library(haven) # example...may replace with any individual package name
```

| website     | description |   
|------------:|:------------|   
| [`broom`](https://github.com/tidymodels/broom) | Convert Statistical Analysis Objects into Tidy Tibbles
| [`haven`](https://haven.tidyverse.org/) | Import and Export **SPSS**, **Stata** and **SAS** Files
| [`hms`](https://github.com/tidyverse/hms) | Pretty Time of Day 
| [`lubridate`](https://lubridate.tidyverse.org/) | Make Dealing with Dates a Little Easier
| [`magrittr`](https://magrittr.tidyverse.org/) | A Forward-Pipe Operator for **$R$** 
| [`glue`](https://github.com/tidyverse/glue) | Interpreted String Literals |
| [`readxl`](https://readxl.tidyverse.org/) | Read **Excel** Files
| [`tibble`](https://tibble.tidyverse.org/) | Simple Data Frames



-------------------------------------

### Groups of Individual Packages on $CRAN$




#### Creating Tables



| website     | description |   
|------------:|:------------|   
| [`furniture`](http://tysonbarrett.com/furniture/)  | Tables for Quantitative Scientists |
| [`pander`](https://rapporter.github.io/pander/)    | An R 'Pandoc' Writer (makes tables look nice) |
| [`stargazer`](https://www.jakeruss.com/cheatsheets/stargazer/) | Well-Formatted Regression and Summary Statistics Tables |
| [`texreg`](https://diffuseprior.wordpress.com/2013/01/20/texreg-a-package-for-beautiful-and-easily-customizable-latex-regression-tables-from-r/)    | Conversion of R Regression Output to LaTeX or HTML Tables |
| [`xtable`](https://cran.r-project.org/web/packages/xtable/vignettes/xtableGallery.pdf) | Export Tables to LaTeX or HTML |
| [`kableExtra`](https://haozhu233.github.io/kableExtra/awesome_table_in_html.html#overview) | Construct Complex Table with `kable` and Pipe Syntax |



#### Visualization




| website     | description |   
|------------:|:------------|     
| [`RColorBrewer`](https://data.library.virginia.edu/setting-up-color-palettes-in-r/) | Color Palettes    |
| [`gghighlight`](https://github.com/yutannihilation/gghighlight) | Highlight Lines and Points in `ggplot2`  |
| [`ggthemes`](https://www.ggplot2-exts.org/ggthemes.html) | Extra Themes, Scales, and Geoms for `ggplot2` |
| [`ggExtra`](https://www.ggplot2-exts.org/ggExtra.html) | Add Marginal Histograms to `ggplot2`, and More `ggplot2` Enhancements  |
| [`ggfortify`](https://github.com/sinhrks/ggfortify) | Data Visualization Tools for Statistical Analysis Results |
| [`ggalt`](https://github.com/hrbrmstr/ggalt) | Lots of extras for `ggplot2` |
| [`GGally`](https://ggobi.github.io/ggally/#canonical_correlation_analysis) | Extension to `ggplot2` |
| [`corrplot`](https://rstudio-pubs-static.s3.amazonaws.com/240657_5157ff98e8204c358b2118fa69162e18.html) | Visualization of a Correlation Matrix |
| `gpairs` | The Generalized Pairs Plot  |
| [`gridextra`](https://cran.r-project.org/web/packages/egg/vignettes/Ecosystem.html) | Miscellaneous Functions for "Grid" Graphics |
| [`likert`](https://github.com/jbryer/likert) | Analysis and Visualization Likert Items |
| [`vcd`](http://www.datavis.ca/courses/VCD/vcd-tutorial.pdf) | Visualizing Categorical Data |
| [`scales`](https://github.com/r-lib/scales) | Scale Functions for Visualization |
| [`cowplot`](https://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html) | Streamlined Plot Theme & Annotations for `ggplot2` |
| [`yarrr`](https://ndphillips.github.io/piratesguide.html) | The Pirate's Guide to $R$ |




#### Generally Handy



| website     | description |    
|------------:|:------------|       
| `polycor` | Polychoric and Polyserial Correlations |  
| [`psych`](http://personality-project.org/r/psych/) | Psychological or Psychometric Procedures |   
| [`corpcor`](http://strimmerlab.org/software/corpcor/) | Covariance and (Partial) Correlation |         
| [`sjlabelled`](https://strengejacke.github.io/sjlabelled/) | Labelled Data Utility Functions |    
| [`sjPlot`](http://www.strengejacke.de/sjPlot/) | Data Visualization for Statistics in Social Science |    
| [`sjmisc`](http://www.strengejacke.de/sjmisc/) | Data and Variable Transformation Functions |    
| [`sjstats`](http://www.strengejacke.de/sjstats/) | Convenient Functions for Common Statistical Computations |        
| [`Hmisc`](http://biostat.mc.vanderbilt.edu/wiki/Main/Hmisc) | Harrell Miscellaneous |    
| [`labelled`](https://github.com/larmarange/labelled) | Manipulating Labelled Data |






#### t-Tests, ANOVA, and RM ANOVA



| website     | description |   
|------------:|:------------|     
| [`afex`](https://github.com/singmann/afex) | Analysis of Factorial Experiments |    
| [`emmeans`](https://github.com/rvlenth/emmeans) | Estimated Marginal Means, aka Least-Squares Means |    
| [`multicomp`](http://multcomp.r-forge.r-project.org/) | Simultaneous Inference in General Parametric Models  | 
| `multcompView` | Visualizations of Paired Comparisons  |




#### Regression (ML, GLM)




| website     | description |   
|------------:|:------------|     
| [`car`](https://www.statmethods.net/stats/rdiagnostics.html) | Companion to Applied Regression |       
| [`effects`](https://www.jstatsoft.org/article/view/v008i15/effect-displays-revised.pdf) | Effect Displays for Linear, Generalized Linear, and Other Models |
| `predictmeans` | Calculate Predicted Means for Linear Models  |





#### Multilevel Models (MLM, HLM, GEE)




| website     | description |   
|------------:|:------------|     
| [`nlme`](http://davidakenny.net/papers/k&h/MLM_R.pdf) | Linear and Nonlinear Mixed Effects Models |    
| [`lme4`](https://github.com/lme4/lme4/) | Linear Mixed-Effects Models |    
| [`lmerTest`](https://github.com/runehaubo/lmerTestR) | Tests in Linear Mixed Effects Models |    
| [`HLMdiag`](https://github.com/aloy/HLMdiag) | Diagnostic Tools for Hierarchical (Multilevel) Linear Models |
| [`geepack`](https://cran.r-project.org/web/packages/geepack/vignettes/geepack-manual.pdf) | Generalized Estimating Equation Package |
| [`gee`](https://cran.r-project.org/web/packages/gee/gee.pdf) | Generalized Estimation Equation Solver |
| [`gee4`](https://github.com/ypan1988/gee4) | Generalised Estimating Equations (GEE/WGEE) |
| [`optimx`](file:///C:/Users/A00315273/Downloads/v43i09.pdf) | A Replacement and Extension of the `optim()` Function |
| [`MuMIn`](https://sites.google.com/site/rforfishandwildlifegrads/home/mumin_usage_examples) | Multi-Model Inference |



#### Structural Equation Modeling (SEM)



| website     | description |   
|------------:|:------------|     
| [`lavaan`](http://lavaan.org) | Latent Variable Analysis |     
| [`OpenMx`](https://openmx.ssri.psu.edu/) | Extended Structural Equation Modelling |   
| [`sem`](https://www.methodsconsultants.com/tutorial/structural-equation-models-using-the-sem-package-in-r/) | Structural Equation Modelling |
| [`semPlot`](http://sachaepskamp.com/semPlot/examples) | Path Diagrams and Visual Analysis of Various SEM Packages' Output  |   





#### Random Forests



| website     | description |   
|------------:|:------------|         
| [`randomForest`](https://www.guru99.com/r-random-forest-tutorial.html) | Random Forests for Classification and Regression |
| [`randomForestSRC`](http://www.riptutorial.com/r/example/13086/random-forest-survival-analysis-with-randomforestsrc) | for Survival, Regression, and Classification |
| [`ggRandomForests`](https://arxiv.org/pdf/1612.08974.pdf) | Visually Exploring Random Forests |
| [`party`](http://party.r-forge.r-project.org/) | A Laboratory for Recursive Partytioning |
| [`partykit`]() | A Toolkit for Recursive Partytioning |




#### Other Models



| website     | description |   
|------------:|:------------| 
| [`mgcv`](https://people.maths.bris.ac.uk/~sw15190/mgcv/tampere/mgcv.pdf) | Mixed GAM Computation Vehicle with Automatic Smoothness Estimation |  
| [`glmnet`](https://web.stanford.edu/~hastie/glmnet/glmnet_alpha.html) | Lasso and Elastic-Net Regularized Generalized Linear Models|
| [`survival`](https://github.com/therneau/survival) | Survival Analysis |
| [`caret`](https://topepo.github.io/caret/index.html) | Classification and Regression Training |





#### Reproducibility and Reporting





| website     | description |   
|------------:|:------------|  
| [`bookdown`](https://bookdown.org/) | Authoring Books and Technical Documents |
| [`blogdown`](https://bookdown.org/yihui/blogdown/) | Create Blogs and Websites|
| [`tidytex`](https://yihui.name/tinytex/) | Helper Functionsfor $TeX Live$, Compile $LaTeX$ Documents |
| [`xaringan`](https://github.com/yihui/xaringan) | Presentation Ninja |

*Note: `slidify` & `ReportRs` have been removed from $CRAN$*



#### REDCap Interface




| website     | description |   
|------------:|:------------|     
| [`redcapAPI`](https://github.com/nutterb/redcapAPI/wiki) | Interface to $REDCap$  |
| [`REDCapR`](https://github.com/OuhscBbmc/REDCapR) | Interaction Between $R$ and $REDCap$ |





#### Creating Your Own Packages




| website     | description |   
|------------:|:------------|  
| [`devtools`](https://github.com/r-lib/devtools) | Tools to Make Developing $R$ Packages Easier|
| [`testthat`](https://github.com/r-lib/testthat) | Unit Testing for $R$ |
| [`roxygen2`](https://cran.r-project.org/web/packages/roxygen2/vignettes/roxygen2.html) | In-Line Documentation for $R$ |




### Installing packages (via syntax code)

Review the list of all the $CRAN packages above:


```r
package_list_tables
```

```
## [1] "furniture"  "pander"     "stargazer"  "texreg"     "xtable"    
## [6] "kableExtra"
```

```r
package_list_visual
```

```
##  [1] "RColorBrewer" "gghighlight"  "ggthemes"     "ggfortify"   
##  [5] "ggalt"        "ggExtra"      "GGally"       "ggeffects"   
##  [9] "corrplot"     "gpairs"       "gridextra"    "likert"      
## [13] "vcd"          "scales"       "cowplot"      "yarrr"
```

```r
package_list_general
```

```
## [1] "psych"      "polycor"    "corpcor"    "sjlabelled" "sjPlot"    
## [6] "sjmisc"     "sjstats"    "Hmisc"      "labelled"
```

```r
package_list_anova
```

```
## [1] "afex"         "emmeans"      "corpcor"      "multicomp"   
## [5] "multcompView"
```

```r
package_list_regression
```

```
## [1] "car"          "effects"      "predictmeans"
```

```r
package_list_multilevel
```

```
## [1] "nlme"     "lme4"     "lmerTest" "HLMdiag"  "geepack"  "gee"     
## [7] "gee4"     "optimx"   "MuMIn"
```

```r
package_list_sem
```

```
## [1] "lavaan"  "OpenMx"  "sem"     "semPlot"
```

```r
package_list_forest
```

```
## [1] "randomForest"    "randomForestSRC" "ggRandomForests" "party"          
## [5] "partykit"
```

```r
package_list_models
```

```
## [1] "mgcv"     "glmnet"   "survival" "caret"
```

```r
package_list_report
```

```
## [1] "bookdown" "blogdown" "tidytex"  "xaringan"
```

```r
package_list_redcap
```

```
## [1] "REDCapR"   "redcapAPI"
```

```r
package_list_package
```

```
## [1] "devtools" "testthat" "roxygen2"
```



Get all the packages from $CRAN$ *(updates if new version available)*:


```r
install.packages(c("tidyverse",
                   package_list_tables,
                   package_list_visual,
                   package_list_general,
                   package_list_anova,
                   package_list_regression,
                   package_list_multilevel,
                   package_list_sem,
                   package_list_forest,
                   package_list_models,
                   package_list_report,
                   package_list_redcap,
                   package_list_package))
```

-------------------------------------

## Other Developmental non-$CRAN$ Packages on $GitHub$

First, make sure you have the `devtools` package installed on your computer *(hint: its in the `package_list_package` list above)*.


```r
install.packages("devtools")
```



### Templates for writing tutorials, practicals or examination papers with $R Markdown$



`unilur` is a $R$ package to help writing tutorials, practicals or examination papers with $R Markdown$.

With `unilur` you can render the following outputs from a single rmarkdown file:

* the exam or tutorial questions (answers remaining hidden) as a PDF or HTML file.

* the exam or tutorial questions with sample answers as a PDF or HTML file.

In addition, you will be able to:

* Create coloured boxes to highlight some markdown or R content.

* Create examination papers with 

    + multiple choice questions
    + a candidate identification form
    + dotted lines placeholders to fill in answers
    
* Create a new $R Markdown$ file with solution chunks replaced by empty ones.

<div class="rmdlink">
<p>Website: <a href="https://github.com/koncina/unilur">GitHub - <code>unilur</code></a> Tutorial: <a href="http://eric.koncina.eu/posts/introducing-the-unilur-rmarkdown-template/">blog post - <code>unilur</code></a></p>
</div>



```r
devtools::install_github("koncina/unilur")
```





### Prepare APA journal articles with $R Markdown$



`papaja` is a $R$ package in the making including a $R Markdown$ template that can be used with (or without) **$R$ Studio** to produce documents, which conform to the **American Psychological Association (APA)** manuscript guidelines (6th Edition). The package uses the $LaTeX$ document class `apa6` and a .docx-reference file, so you can create PDF documents, or Word documents if you have to. Moreover, papaja supplies $R$ functions that facilitate reporting results of your analyses in accordance with APA guidelines.

`papaja` has not yet been submitted to $CRAN$ because it is under active development. Currently, there are still a couple of loose ends they would like to tie up before we release the package to a larger audience.  There are two versions you can install from the $GitHub$ website.


<div class="rmdlink">
<p>Website: <a href="https://github.com/crsh/papaja">GitHub - <code>papaja</code></a> Tutorial: <a href="https://crsh.github.io/papaja_man/">eBook - <code>papaja</code></a></p>
</div>



```r
# Install the stable development verions from GitHub
devtools::install_github("crsh/papaja")

# Install the latest development snapshot from GitHub
devtools::install_github("crsh/papaja@devel")
```







