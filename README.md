# Data Analytics Assignment (R Markdown)

This repository contains a university data analytics assignment written in **R Markdown**. It covers end-to-end analysis across two themes:
- **COVID-19 dataset**: cleaning, feature preparation, exploratory analysis, visualisation, and predictive modelling.
- **Used-car datasets**: dataset justification, data wrangling/standardisation, and merging multiple car listing files for analysis-ready data.

## What's included

### Section 1 (COVID-19)
- `assignment_final_task1.Rmd` — Imports raw data, cleans/transforms, and produces cleaned outputs.
- `assignment_final_task2.Rmd` — Visual exploration and charts.
- `assignment_final_task3.Rmd` — Data-driven modelling (e.g., linear regression, ridge/lasso regularisation, decision trees).
- `assignment_final_task4.Rmd` — Communication-focused write-up (including audience/accessibility considerations).

### Section 2 (Used-car data)
- `assignment_fina_section2.Rmd` — Dataset justification + wrangling, standardisation, and merging multiple car datasets.

## Data files expected
The Rmd files reference these CSVs (place them in the same folder as the Rmds, or update paths in the code):
- `covid19_clean.csv` (generated in Task 1, then used in Tasks 2–3)
- `lastDay_data.csv` (generated in Task 1)
- `CAR DETAILS FROM CAR DEKHO.csv`
- `Car details v3.csv`
- `car details v4.csv`
- `car data.csv`

> If you prefer a cleaner structure, create a `/data` folder and update file paths in the Rmds.

## Tools & packages
Recommended setup:
- R (latest stable)
- RStudio
- R Markdown / knitr

Commonly used packages across the analysis include:
- `tidyverse` (dplyr, tidyr, ggplot2, readr)
- `lubridate` (dates)
- `glmnet` (ridge/lasso)
- `caret` (modelling workflow)
- plus other supporting packages referenced inside each Rmd

## How to run
1. Open the project folder in **RStudio**.
2. Install missing packages when prompted (or install manually).
3. Open any `.Rmd` file and click **Knit** to generate HTML/PDF output.

Example (optional) install snippet:
```r
install.packages(c(
  "tidyverse", "lubridate", "knitr", "rmarkdown", "glmnet", "caret"
))
