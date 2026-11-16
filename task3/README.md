# Messy Customer Sales Data Cleaning & Preprocessing

## 📌 Project Overview

This project focuses on cleaning and preprocessing a highly inconsistent Customer Sales dataset using Python.

The dataset contained multiple data quality issues, including missing values, inconsistent categorical formats, duplicate records, invalid age entries, outliers and incomplete customer information.

The primary objective was to improve data quality while retaining as much meaningful information as possible.

## 📂 Dataset Information

- **Initial Records:** 10,200
- **Total Columns:** 12
- **Domain:** Customer & Sales Data

### Dataset Attributes
- Customer_ID
- Name
- Gender
- Age
- City
- Signup_Date
- Last_Purchase_Date
- Purchase_Amount
- Feedback_Score
- Email
- Phone_Number
- Country

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## 🔍 Data Cleaning Process

### 1. Initial Data Inspection
- Examined dataset structure, dimensions and data types.
- Identified missing values across multiple columns.
- Checked duplicate records and inconsistent entries.
- Created a copy of the original dataset for comparison.

### 2. Handling Inconsistent Data
- Standardized Gender values into consistent categories (`m`, `f`).
- Cleaned inconsistent capitalization and spacing in City and Country columns.
- Standardized country entries, including correcting `Ind` to `India`.
- Converted Age values containing text such as `51 years` into numeric format.
- Converted date columns into appropriate datetime formats.
- Cleaned whitespace in Email entries.

### 3. Duplicate Removal
- Identified and removed duplicate records to maintain data consistency.

### 4. Age Analysis & Outlier Detection
- Used KDE plots to understand the age distribution.
- Applied the Interquartile Range (IQR) method for outlier detection.
- Used Z-score analysis as an additional statistical check.
- Examined mean, median, standard deviation, skewness and kurtosis.
- Removed identified age outliers and invalid non-positive age values.

### 5. Missing Value Analysis & Treatment
This was one of the most challenging parts of the project.

Instead of applying a single imputation strategy to every column:

- Analyzed missing values across Gender, Age, City and other attributes.
- Used city-level and demographic analysis to investigate missing values.
- Explored gender-wise age distributions.
- Applied selective median-based age imputation.
- Investigated unknown demographic information before making cleaning decisions.
- Removed selected records where multiple important attributes were simultaneously missing and reliable recovery was not possible.

### 6. Final Validation
- Rechecked missing values after cleaning.
- Verified data types.
- Removed remaining duplicate records.
- Compared the original and processed datasets.

## 📊 Before vs After

| Metric | Before | After |
|---|---:|---:|
| Total Records | 10,200 | 8,944 |
| Columns | 12 | 12 |
| Duplicates | 15 | 0 |
| Missing Values | 7,804 | 2,672 |

*Missing-value counts are based on the notebook's initial and final inspection calculations.*

## 📈 Key Observations

- The dataset contained substantial missing information across customer attributes.
- Gender and City columns required categorical standardization.
- Age required extensive preprocessing due to mixed data formats, missing values and outliers.
- City-wise demographic analysis helped guide selective imputation decisions.
- Not every missing value could be reliably recovered, so some missing values were retained rather than introducing unsupported assumptions.

## 🎯 Key Learnings

- Handling real-world messy datasets requires more than basic Pandas operations.
- Statistical analysis can help identify unusual observations.
- Missing value treatment should consider the context of individual columns.
- Data cleaning decisions involve balancing data retention and data reliability.
- Understanding the dataset before applying transformations is essential.

## 📁 Project Structure

```text
Messy-Customer-Sales-Data-Cleaning/
│
├── main.ipynb
├── messy_customer_sales_data.csv
├── cleaned.csv
└── README.md
```

## 🚀 Conclusion

This project provided hands-on experience in handling real-world data quality challenges, performing exploratory analysis, applying statistical techniques and making context-driven preprocessing decisions.

The focus was not simply to make the dataset look clean, but to make informed decisions about data quality and reliability.
