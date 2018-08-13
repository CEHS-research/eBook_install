# Data Management

How do you get data into R, view and work with in, and then save it for later use.


-----------

## Importing Data From Various Formats

### Text Format (.csv, tab-delimited, ect.)

Use `read.csv()`

### Excel Format (.xls, .xlsx)

Use `haven::read.spss()`


### SPSS Format (.sav)

Use `readxl::read.excel()`


### REDCap (API directly)


-----------

## Viewing Data Within R Studio


### The Environment Tab

### Notebook Display








-----------

## Saving Data in R Format


Use `save(..., file = "name.RData")`
