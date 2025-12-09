# Tech Students and Mental Health

## What is this GitHub repository all about?

This repository contains all of the code and supporting files for our Intermediate Data Science final project on **Tech Students and Mental Health**.
Using survey data from primarily STEM students, we:
- Created exploratory visualizations
- Quantify relationships between academcic workload/pressure and mental health outcomes (e.g., depression, anxiety, isolation, future insecurity) 
- Produce a final report and presentation-ready figures summarizing key findings 

The goal is to provide a reproducible workflow from raw data to final visualizations and summary statistics.


## Software requirements (with versions)

To run the code in this repository, you will need:

- **R**: version **4.4.3** or later  
- **RStudio**: version **2025.05.1+513** or later  

We recommend updating to a recent version of R and RStudio if you encounter any issues.

## Required R packages

The analysis uses the following R packages:

```r
library(tidyverse)
library(janitor) 
library(viridisLite)
library(stringr)
library(readr)
library(skimr)
library(psych)
library(GGally)
library(extrafont)
library(showtext)
library(ggcorrplot)
library(dplyr)
library(purrr)
library(grid)
library(patchwork)
library(ggh4x)
```

# What does the expected output look like?

When everything runs correctly, you should see:
- Cleaned analytic dataset
- A processed data file saved to data
- Variables with readable names and consistent formats (thanks to janitor, dplyr, and stringr)
Key visualizations
- A correlation heatmap (using ggcorrplot and/or GGally) showing how academic workload and academic pressure variables relate to mental health outcomes
- Boxplots / violin plots comparing mental health scores across different levels of predictor variables
- Combined figure layouts using patchwork and ggh4x for multi-panel displays
- Summary output in the report
- Descriptive statistics (means, SDs) for key variables
Final report / slides
- An HTML report and/or slides that includes:
- Research question and motivation
- Methods and variables used
- Main visualizations (e.g., heatmaps, plots)
- Brief interpretation of how academic and other factors relate to mental health among college students

Reproducibility notes
- All paths are written relative to the project root (set automatically when you open the .Rproj file in RStudio).
- If you change the folder structure or file names, update the paths in the scripts accordingly.
- If you run into font-related issues with extrafont or showtext, you can temporarily switch to default fonts or re-run font installation/import commands described in the code comments.
