# V-S-Date

## V&S Survey Data Analysis Repository

This repository contains data files, R Markdown scripts, and outputs related to the analysis of the V&S survey datasets. It is organized to facilitate the processing, cleaning, and analysis of survey data for morning, evening, and EMA surveys.

## Repository Structure

### Data Files

SMS Data.09.03.24.xlsx: Contains SMS StusyID data.

V&S 3Hours EMA Survey_September 30, 2024_17.00.csv: EMA survey data.

V&S Baseline Survey_September 9, 2024_10.27.csv: Baseline survey data.

V&S Evening Survey_September 30, 2024_17.01.csv: Evening survey data.

V&S Morning Survey_September 30, 2024_17.01.csv: Morning survey data.

survey_count_long_filtered.csv: Filtered survey counts for all duplication analysis.

### R Markdown Scripts

V&S Data Baseline Missing.Rmd: Script for analyzing and identifying missing data in the baseline survey.

V-S-EMA-Missing-.Rmd: Script for analyzing missing data in EMA surveys, including a recent restart for December.

### Outputs

V-S-Data-Baseline-Missing.html / .pdf: HTML and PDF outputs summarizing missing data in the baseline survey.

V-S-EMA-Missing-.html: Output detailing missing data in the EMA, morning, and evening surveys.

morning_duplicates_diff.html / .xlsx: Analysis of duplicate records in morning survey data.

ema_duplicates.xlsx, evening_duplicates.xlsx, morning_duplicates.xlsx: Excel files containing duplicate analysis for different survey.

### Project Files

V-S-Data.Rproj: RStudio project file for the analysis.

.gitignore: Specifies files and directories ignored by Git.

## Getting Started

Prerequisites

Ensure you have the following installed:

R (version 4.0 or above)

Required R packages: dplyr, tidyr, readr, openxlsx, and rmarkdown


## Notes

All missing data are coded:
Recode seen but unanswered questions as -99
Recode seen but unanswered multi-value fields as -999
using -98 (skip logic) and -97 (don't know).



