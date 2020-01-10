# A Practical Guide to Reproducible Papers [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ablucher/Workshop_ReproduciblePaper/master?urlpath=rstudio)

Binder let's us capture the exact R environment we used for our analysis. Using binderHub, we can host our R markdown notebook inside an RStudio session in the cloud, which allows users to recreate or modify our analysis. Any changes users make won't be saved; modifications have to be made on our end through repository commits. 

# What we need

## GitHub Repository (make sure it's public!)

## R markdown notebook
Create your R markdown notebook as usual! But keep track of your libraries, as we will need to tell binder to install all our needed packages.

In our example script, we just read in a simple data set, do some filtering, and create a barplot.

## Configuration for Binder
We need to include two additional files in our repository to get set up for binder. 

### runtime.txt
The [runtime.txt](https://github.com/ablucher/Workshop_ReproduciblePaper/blob/master/runtime.txt) file is where we specify our R environment (R version) using the following syntax:

r-YYYY-MM-DD

### install.R 
The [install.R](https://github.com/ablucher/Workshop_ReproduciblePaper/blob/master/install.R) is where we specify all our packages need to run our R markdown. For instance, here we need 'knitr', 'rmarkdown', 'dplyr', 'ggplot2' and 'here'. 

# Acknowledgements
This work was supported by OHSU's BioData Club, and the following grant:
BioData Club: A Partnership Model for Data Management and Data Science Education, NLM UG4LM012344
