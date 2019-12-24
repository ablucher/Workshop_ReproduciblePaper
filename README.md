# Workshop_ReproduciblePaper
A Practical Guide to Reproducible Papers [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ablucher/Workshop_ReproduciblePaper/master?urlpath=rstudio)

Hands-on component. Binder let's us capture the exact R environment we used for our analysis. We can also create an RStudio session to that future users can re-run and modify our analysis. 

Here's what we need:

# R markdown file
Create your R markdown file as usual! But keep track of your libraries, as we will need to tell binder to install all our needed packages in the install.R file.

In our example script, we just read in a simple data set, do some filtering, and create a barplot.

# runtime.txt
This file is where we specify our R environment (R version) using the following syntax:
r-YYYY-MM-DD

You can access a full list of R versions [here].

# install.R 
This file is where we specify all our packages need to run our R markdown. For instance, here we need 'knitr', 'rmarkdown', and 'tidyverse'. 
