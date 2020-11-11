# Supporting Information

This repository holds all supplementary source code needed to reproduce the calculations and plots of the following manuscript: 

**Asamoto CK, Rempfert KR, Luu VH, Younkin AD, Sigman DM, Kopf SH. Enzyme specific isotope effects of the Nap and Nar nitrate reductases. *In Review*.**

The fully compiled analysis files are available as [HTML reports](https://www.kopflab.org/2020_asamoto_et_al/). For the easiest way to run the source [R Markdown](http://rmarkdown.rstudio.com/) (.Rmd) files that produce these HTML reports yourself along with the data figures in PDF and PNG format and the data tables in XLSX format, please follow the instructions below.

## What is R Markdown?

[R Markdown](http://rmarkdown.rstudio.com/) is a so-called "literate programming" format that enables easy creation of dynamic documents with the [R](http://www.r-project.org/) language. HTML and PDF reports can be generated from R Markdown files using [knitr](http://yihui.name/knitr/) and [pandoc](http://johnmacfarlane.net/pandoc/), which can be installed automatically with [RStudio](http://www.rstudio.com/), and are fully integrated into this cross-platform IDE. All software used for these reports (R, RStudio, etc.) is freely available and completely open-source. 

## How can I run this code?

### Option 1: Run it in the cloud using [binder](https://mybinder.org/)

1. Use the following links to load this entire repository and all its dependencies in an online RStudio or Jupyter Lab instance (note that these may take a few minutes to launch):
   - [![RStudio Binder](https://img.shields.io/badge/explore%20online-in%20RStudio-blue.svg)](http://beta.mybinder.org/v2/gh/kopflab/2020_asamoto_et_al/master?urlpath=rstudio)
   - [![Jupyter Binder](https://img.shields.io/badge/explore%20online-in%20Jupyter-orange.svg)](http://beta.mybinder.org/v2/gh/kopflab/2020_asamoto_et_al/master?urlpath=lab)
1. In the online RStudio: open and work with any of the R Markdown (.Rmd) files in the file browser. You can generate an HTML report ("knit HTML") by selecting File --> Knit from the menu. The HTML report will be displayed upon successful completion and is saved as a standalone file in the same directory (these are the files made [available online](https://www.kopflab.org/2020_asamoto_et_al/)). All generated data figures are saved as PDF and PNG in the `figures` sub-directory. All generated data tables are saved as XLSX in the `tables` sub-directory.
1. In the online Jupyter lab: open and work with any of the notebook (.ipynb) files in the file browser. 
1. Make sure to download any edited or generated files you want to keep. They will disappear once you close the binder instance (or once it gets terminated due to inactivity).

### Option 2: Run it on your desktop

The quickest and easiest way is to use RStudio.

 1. Download and install [R](http://cran.rstudio.com/) for your operating system
 1. Download and install [RStudio](http://www.rstudio.com/products/rstudio/download/) for your operating system
 1. Download a [zip file of this repository](https://github.com/KopfLab/2020_asamoto_et_al/archive/master.zip) and unpack it in an easy to find directory on your computer
 1. Navigate to the directory and double-click the `project.Rproj` file to start RStudio and load this project.
 1. Install the required libraries by running the following command in the Console in RStudio: `install.packages(c("tidyverse", "latex2exp", "cowplot", "broom", "phangorn", "openxlsx", "BiocManager"))` followed by `BiocManager::install("ggtree")` or by installing them manually in RStudio's Packages manager.
 1. Open any of the R Markdown (.Rmd) files in the file browser
 1. To generate an HTML report ("knit HTML"), select File --> Knit from the menu. The HTML report will be displayed upon successful completion and is saved as a standalone file in the same directory (these are the files made [available online](https://www.kopflab.org/2020_asamoto_et_al/) and linked in the SI). All generated data figures are saved as PDF and PNG in the `figures` sub-directory. All generated data tables are saved as XLSX in the `tables` sub-directory.
 
## What can I do with this code?

We hope that this code, or any part of it, might prove useful to other members of the scientific community interested in the subject matter. All code is completely open-access and can be modified and repurposed in every way. If significant portions are reused in a scientific publication, please consider citing our work. Please make sure to cite this work if re-using any of our data.

## Troubleshooting notes

The R Markdown files in this repository make use of various R modules for data processing, plotting and modelling. All of these should be installed automatically when the first R Markdown file is knitted (if the knitting fails because of a missing package, please install it manually, an error will indicate which package could not be installed). 
