Employee Turnover Data Profiling and Cleaning
Project Overview

This project focuses on profiling, inspecting, and cleaning an employee turnover dataset for a large multinational technology firm. The goal is to prepare a high-quality, analysis-ready dataset that can be used for exploratory analysis and predictive modeling related to employee turnover.

The project was completed as part of a data preparation and exploration task and demonstrates the use of Python and pandas to identify and resolve common data quality issues.

Objectives

The primary objectives of this project are to:

Inspect the dataset for data quality issues

Identify duplicate records, missing values, inconsistent entries, formatting errors, and outliers

Apply appropriate data cleaning techniques using Python

Create and export a cleaned version of the dataset in CSV format

Document the process in a clear, reproducible manner

Dataset Description

Unit of analysis: One row represents one employee

Data types: Combination of numerical and categorical variables

Key variables include:

Employee demographics (e.g., age, gender, marital status)

Job and compensation details

Professional development information

Employee turnover indicator

⚠️ The raw dataset is not included in this repository due to privacy and academic integrity requirements.

Tools and Technologies

Python

pandas

NumPy

Operating System: Windows (paths may need adjustment on macOS/Linux)

Data Quality Issues Inspected

The dataset was inspected for the following issues:

Duplicate Entries

Full-row duplicate records were identified using pandas’ duplicated() function.

Missing Values

Missing values were summarized by column to identify incomplete variables.

Inconsistent Entries

Categorical variables were examined for inconsistent formatting (e.g., underscores vs. spaces).

Formatting Errors

Column name whitespace and numeric values stored as text (e.g., currency symbols) were identified.

Outliers and Invalid Values

Descriptive statistics and logic-based checks were used to detect invalid values such as negative salaries or commuting distances.

Data Cleaning Approach

After inspection, the following cleaning steps were applied:

Removed full-row duplicate records

Converted numeric-looking text columns to numeric data types

Replaced invalid negative values with missing values

Imputed missing numeric values using the median

Filled missing categorical values with "Unknown"

Standardized categorical labels for consistency

Preserved as much valid data as possible while ensuring reliability

How to Run the Script

Clone this repository:

git clone https://github.com/your-username/employee-turnover-data-cleaning.git


Open the Python script and update the dataset path:

DATA_PATH = r"C:\path\to\Employee Turnover Dataset.csv"


Run the script:

python employee_turnover_cleaning.py


When prompted, enter the folder where you want the cleaned dataset saved.

The cleaned file will be exported as:

Employee_Turnover_Cleaned.csv

Output

Employee_Turnover_Cleaned.csv

Duplicate-free

Consistent categorical values

Valid numeric values

Ready for analysis and modeling

Notes

This project intentionally avoids reliance on employee identifiers for deduplication and instead focuses on full-row duplicates.

The script is modular and readable to support academic review and reproducibility.

All cleaning decisions are documented and aligned with data preparation best practices.
