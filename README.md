# SWYNEX – Data Cleaning & Preparation

## Project Overview
This project focuses on cleaning and preparing the Titanic dataset using Python and Pandas. The main objective is to identify missing values, analyze duplicate records, validate data, and prepare a clean dataset for further analysis.

## Internship Details
- **Company:** SWYNEX Technologies
- **Domain:** Data Analyst
- **Task:** Task 1 – Data Cleaning & Preparation
- **Internship ID:** SWX-2026-003440

## Tools & Technologies
- Python
- Pandas
- NumPy
- VS Code

## Dataset Information
- **Dataset:** Titanic Dataset
- **Source:** [Seaborn Titanic Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/titanic.csv)
- **Total Records:** 891
- **Total Columns:** 15

## Data Cleaning Process

### 1. Missing Values Analysis
Identified missing values in the following columns:

| Column | Missing Values |
|---|---:|
| age | 177 |
| embarked | 2 |
| deck | 688 |
| embark_town | 2 |

### 2. Missing Values Handling
- Filled missing values in `age` using the median (28.0).
- Filled missing values in `embarked` using the mode (S).
- Filled missing values in `embark_town` using the mode (Southampton).
- Kept missing values in `deck` because approximately 77.21% of its values were missing.

### 3. Duplicate Records Analysis
- Identified 107 duplicate rows before handling missing values.
- After filling missing ages, 110 exact duplicate rows were identified.
- Duplicate records were not removed because identical records do not necessarily represent the same passenger. The dataset does not provide a unique passenger identifier.

### 4. Data Validation
Performed the following validation checks:

| Validation | Invalid Records |
|---|---:|
| Invalid Age | 0 |
| Negative Fare | 0 |
| Invalid Passenger Class | 0 |
| Invalid Survival Values | 0 |
| Invalid Gender | 0 |

All five validation checks passed.

## Final Dataset
- **Total Records:** 891
- **Total Columns:** 15
- Missing values in `age`, `embarked`, and `embark_town` were handled.
- Original raw data was preserved.
- Cleaned dataset was exported as a CSV file.

## Project Files
- `data_cleaning.py` – Python data cleaning script.
- `data/titanic_raw.csv` – Original dataset.
- `data/titanic_cleaned.csv` – Cleaned dataset.
- `README.md` – Project documentation.

## Conclusion
Successfully completed the data cleaning and preparation process using Python and Pandas. The cleaned dataset is now ready for further exploratory data analysis.

**Project completed as part of the SWYNEX Technologies Data Analyst Internship.**