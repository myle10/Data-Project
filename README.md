# Data Exploration Project

**Author:** : Nick Huntington-Klein
**Date:** 2023-12-14

## Overview

Welcome to Data Exploration Project! This repository contains all the materials for the Data Exploration Project. The objective is to analyze the influence of the College Scorecard's release on student interest in higher-earning colleges as indicated by Google search trends and median earnings data.

## Data

Contained within `Data_Exploration_Rawdata.zip` are several CSV files crucial for the analysis:

1. **Google Trends Data (`trends_up_to_....csv`)**: These files capture the index of search terms associated with U.S. universities across different time frames.

2. **College Scorecard Data (`Most+Recent+Cohorts+(Scorecard+Elements).csv`)**: A dataset from the College Scorecard providing detailed information on U.S. colleges and their graduates.

3. **Linking File (`id_name_link.csv`)**: This file facilitates matching identifiers between the Scorecard and Google Trends datasets.

## Research Question

**Did the release of the College Scorecard in September 2015 shift student interest toward colleges with higher graduate earnings, as reflected in the volume of Google searches for related keywords?**

## Analysis

The analysis will involve statistical regression and graphical representation to dissect the trend changes. Decisions on data categorization and level of analysis will be detailed, along with the design rationale for the regression model.

1. **Defining "High-Earning" and "Low-Earning" Colleges**: You will need to decide how to categorize colleges as "high-earning" and "low-earning." This choice should be explained and justified in your analysis.

2. **Data Level**: Determine the level at which the data should be analyzed. You can keep the data as is, with one row per week per keyword, or aggregate it by grouping and summarizing, e.g., one week per college, one month per college, or one month per keyword. Explain your choice.

3. **Regression Model Design**: Design your regression model to address the research question. Consider transformations, functional forms, standard error adjustments, and how to interpret the results.

## Important Project Notes

- `/data`: Raw data files.
- `/scripts`: R scripts for data cleaning (`cleaning.R`) and analysis (`analysis.R`).
- `/docs`: Analysis report in Quarto format (`report.qmd`) and its rendered output.

## The Writeup

To replicate the study:

1. Clone this repository to your local machine.
2. Install R and the required libraries (`tidyverse`, `readr`, `rio`, etc.).
3. Execute the R scripts in `/scripts` sequentially.
4. Review the analysis in `/docs` for the detailed findings.

## Considerations

- Anticipate time for meticulous data preparation and potential iterative corrections.
- Align all analyses with the central research inquiry.
- Interpretations of the results should be precise and linked to the research question.

## Documentation

Your report should be an RMarkdown document that walks through the analysis, justified methodologies, and findings.

## Your Project

Ensure the GitHub repository is well-organized, with a clear file structure, and includes:

- A folder for raw data (`/data`).
- A folder for R scripts (`/code`).
- A folder for cleaned or processed data (`/processed_data`).

Notes about your code:

- Do not include large raw data files in the repository. Instead, store processed data outputs.
  
- When knitting your document, ensure that all code chunks are set to be visible. This transparency is vital for reproducibility and peer review.

- It is advisable to modularize your project by separating the data preparation and analysis into distinct R scripts. This approach enhances readability and maintenance of the code.

- Always utilize relative file paths in your scripts to reference data files and other resources. This practice ensures that your project is portable and can be run on any machine without modification to the code.

- To consolidate the Google Trends CSV files (`trends_up_to_*.csv`), leverage the `import_list()` function from the `rio` package, setting the `rbind=TRUE` parameter. This function will efficiently combine the data into a single dataframe.


## Grading Rubric

The project will be graded on the following:

- Adherence to submission guidelines (5%).
  
- Thoroughness of data cleaning (20%).
  
- Analytical choices and justifications (25%).
  
- Accuracy in interpreting the results (20%).
  
- Overall conclusions about the research question (20%).
  
- Writing clarity and engagement (10%).

This project is your chance to showcase your ability to turn raw data into meaningful insights. Good luck, and may your findings be insightful!
