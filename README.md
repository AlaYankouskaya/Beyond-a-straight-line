# Beyond-a-straight-line
This repository contains all the analysis scripts and visualizations associated with the manuscript submitted to *Nature Human Behaviour*. To ensure full reproducibility, this README provides detailed setup instructions.
This repository provides custom codes to replicate the results of our study. 

GENERAL INFORMATION ABOUT THE STUDY
Abstract:
As social media becomes increasingly embedded in daily life, understanding the relationship between its positive and problematic use has become a global priority. Using data from the 2023 Global Digital Wellbeing Survey (N = 30,994 across 35 countries), we investigated how symptoms of Social Media Disorder (SMD) relate to social media-related well-being (SMWB) measured across dimensions of PERMA model. Both constructs showed substantial cross-national variation, however, the different rates of SMD were not consistently associated with certain rates of poor SMWB suggesting that the relationship between the problematic and positive social media use is neither linear nor globally uniform. We applied latent profile analysis to identify distinct configurations defined by specific combinations of SMD symptoms and SMWB scores. These profiles were structurally consistent across regions, suggesting shared global patterns in how individuals experience social media. At the same time, their prevalence across regions varied significantly, reflecting sociocultural differences in how SMD and SMWB co-occur. The findings challenge severity-based models that treat problematic use as universally associated with diminished well-being on social media and highlight the need to study both problematic and positive use without assuming a straightforward negative relationship between them. Therefore, solutions for digital well-being and social media addiction should address this relationship, while also taking into account the cultural and regional context.

Research questions addressed in the present study:
Are all patterns of SMD symptoms equally detrimental to SMWB? How are distinct SMD symptom profiles associated with differences in SMWD? And to what extent do these psychological patterns differ across world regions, reflecting culturally embedded differences in digital life and well-being?

Hypotheses tested in the present study:
1.	There are distinct and replicable psychological profiles defined by patterns of social media disorder symptoms (SMD) and social media-related well-being (SMWB)
2.	These psychological profiles differ meaningfully in both the expression of SMD symptoms and levels of SMWB across the five PERMA domains.
3.	The latent profile structure, defined by patterns of SMD symptoms and SMWB domains remains consistent across world regions, indicating structural invariance.
4.	Despite structural consistency, the prevalence of SMD-SMWB profiles varies markedly across global regions, reflecting different prevalence rates of these profiles

HOW TO RUN THE ANALYSES
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





