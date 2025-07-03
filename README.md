# Beyond-a-straight-line
This repository contains all the analysis scripts and visualizations associated with the manuscript submitted to *Nature Human Behaviour*. To ensure full reproducibility, this README provides detailed setup instructions.
This repository provides custom codes to replicate the results of our study. 

Install R and RStudio:
If you haven't already: Download and install **R**: https://cran.r-project.org/
Download and install **RStudio** (recommended): https://posit.co/download/rstudio-desktop/

Install Required R Packages (use the following code prior any analyses:
```r
# Install core CRAN packages
install.packages(c(
  "readr",       # For reading CSV files
  "readxl",      # For reading Excel files
  "openxlsx",    # For writing Excel files
  "stringr",     # For string operations
  "dplyr",       # For data manipulation
  "tidyr",       # For reshaping data
  "ggplot2",     # For visualizations
  "viridis",     # For color scales
  "forcats",     # For factor manipulation
  "tidyLPA",     # For latent profile analysis
  "mice",        # For multiple imputation
  "psych",       # For exploratory factor analysis
  "lavaan",      # For confirmatory factor analysis
  "Rtsne",       # For t-SNE visualization
  "patchwork"    # For combining ggplot2 plots
))

Once packages are installed, open any .Rmd or .R file in RStudio and press Ctrl+Shift+Enter (or Cmd+Shift+Enter on Mac) to run the code:
Each script is self-contained and heavily commented to guide you through what it does.

EXAMPLE: For Demographic plots:
Open RStudio
Load and run this R Markdown file:
rmarkdown::render("demographic_plots.Rmd")





