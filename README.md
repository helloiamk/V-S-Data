# V-S-Date

# Overview
This script cleans and processes data from two datasets: SMS Data and V&S Baseline Survey. It identifies missing or mismatched StudyIDs, cleans participation data, and handles missing or "Don't know" responses.

# Datasets
SMS Data: SMS Data.09.03.24.xlsx (Study participation data)
V&S Baseline Survey: V&S Baseline Survey_September 9, 2024_10.27.csv (Survey responses)

# Steps
Load Libraries: Import readxl, dplyr, readr, and tidyr for data manipulation.
Read & Filter SMS Data:
Filter Participation Status = Done and Study Status = Complete/Compensation Sent.
Extract unique StudyIDs.
Read & Clean V&S Baseline Data:
Remove invalid or missing StudyIDs, filter finished == True, and match StudyIDs from SMS Data.
Check Missing/Extra IDs:
Identify StudyIDs missing from V&S Baseline and vice versa.
Data Cleaning:
Drop unnecessary columns.
Recode missing values as -98 and "Don't know" responses as -97.
