# Workshop_ReproduciblePaper
A Practical Guide to Reproducible Papers [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ablucher/Workshop_ReproduciblePaper/master?urlpath=rstudio)

Binder let's us capture the exact R environment we used for our analysis. Using binderHub, we can host our R markdown notebook inside an RStudio session in the cloud, which allows users to recreate or modify our analysis. Any changes users make won't be saved; modifications have to be made on our end through repository commits. 

# What we need

## GitHub Repository (make sure it's public!)

## R markdown file
Create your R markdown file as usual! But keep track of your libraries, as we will need to tell binder to install all our needed packages.

In our example script, we just read in a simple data set, do some filtering, and create a barplot.

## DOCKER file
Here, we set up using a DOCKER file, which can be found in the binder folder. 


# Option 2. Alternate set up for binder
Instead of using a DOCKER file, we can set up our repository using a runtime.txt file and an install.R file. 

# runtime.txt
This file is where we specify our R environment (R version) using the following syntax:
r-YYYY-MM-DD

You can access a full list of R versions [here].

# install.R 
This file is where we specify all our packages need to run our R markdown. For instance, here we need 'knitr', 'rmarkdown', and 'tidyverse'. 

