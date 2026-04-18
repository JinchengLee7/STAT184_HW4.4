# UCI Wine Quality Regression Analysis

This repository contains a reproducible **R and Quarto** project that studies the **UCI Wine Quality** dataset through regression analysis. The main purpose of the project is to examine how physicochemical properties of wine, such as acidity, density, sulphates, and alcohol, relate to the response variable `quality`, and to communicate those findings in a clear and reproducible report.[1]

The project uses the **UCI Wine Quality** dataset from the **UCI Machine Learning Repository**. UCI describes this dataset as suitable for both **classification and regression**, and identifies `quality` as the target variable measured on a score from 0 to 10.[1] In this repository, the analysis report is stored in a Quarto source file named **`analysis-report.qmd`**.

## Project Description

The analysis is designed as a practical regression case study. The report begins with a short description of the dataset, then explores the variables through summary statistics and visualizations, and finally fits one or more regression models to predict wine quality from the available chemical measurements. The main deliverable is a Quarto report that can be rendered into PDF.

The broader purpose of the repository is to show not only statistical work, but also good research workflow. For that reason, the repository includes source files, a final output file, and supporting project documentation.

## Data Source

The data come from the **Wine Quality** dataset hosted by the **UCI Machine Learning Repository**.[1] In the repository structure you showed, the raw dataset consists of **three files** stored in `data/raw/`:

| File | Purpose |
|---|---|
| `data/raw/winequality-red.csv` | Red wine quality observations |
| `data/raw/winequality-white.csv` | White wine quality observations |
| `data/raw/winequality.names` | Dataset description and variable notes |

This layout supports the reproducibility requirement because the analysis can refer to files that are stored directly inside the repository rather than on a private local machine. The report should therefore use **relative paths** such as `data/raw/winequality-red.csv` and `data/raw/winequality-white.csv`.

## What This Repository Contains

The repository is organized to make the project easy to follow and reproduce.

| File or folder | Purpose |
|---|---|
| `README.md` | Introduces the project and explains the repository at a high level |
| `PLAN.md` | Stores the separate execution and repository-management plan |
| `analysis-report.qmd` | Main Quarto source file for the regression analysis |
| `output/` | Stores the rendered report output, such as the final PDF |
| `data/raw/` | Stores the raw UCI wine dataset files |
| `data/processed/` | Stores optional cleaned or combined datasets |
| `R/` | Stores optional helper functions |
| `figs/` | Stores figures used in the report |

## Expected Analysis Workflow

The report is expected to load the raw data files, describe the variables, fit a regression model, and interpret the results in narrative form. Depending on the project design, the report may analyze the red wine file, the white wine file, or a carefully combined dataset created from both files. In each case, the final document should contain section headings, explanatory text, labeled code chunks, and a rendered PDF output.

The source document is written in Quarto so that the analysis and the written explanation stay together in one reproducible file. For consistency with the repository structure, the report file should be named **`analysis-report.qmd`**.

## Reproducibility

This project is intended to be self-contained. Required files should remain inside the repository, and the Quarto document should use relative file paths instead of absolute local paths. The final PDF report should also be stored in the repository so that the completed output is directly visible.

## Contact Information

Name: **Jincheng Li**  
Email: **jfl6553@psu.edu**
Class: **STAT 184, 26SP, Taught by Shubo Li**

## References

[1]: https://archive.ics.uci.edu/dataset/186/wine+quality "Wine Quality - UCI Machine Learning Repository"