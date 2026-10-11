# Task 1: Exploratory Data Analysis on Retail Sales Data

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on a retail sales dataset to identify sales patterns, understand customer behaviour, analyze product performance, and generate actionable business insights.

The analysis uses Python's data analysis and visualization libraries to explore the dataset, uncover trends, and support data-driven business decisions.

## Objectives

- Inspect the dataset's structure, data types, and missing values.
- Calculate descriptive statistics for numerical variables.
- Analyze monthly and quarterly sales trends.
- Explore customer demographics, including age groups and gender distribution.
- Identify the top 10 best-selling products.
- Compare revenue across product categories.
- Visualize correlations between numerical variables.
- Discover additional patterns through exploratory visualizations.
- Provide actionable business recommendations based on the findings.

## Tech Stack

- **Python** — Data analysis and processing
- **Pandas** — Data manipulation and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Jupyter Notebook** — Interactive analysis and documentation

## Project Structure

```text
Oasis-Infobyte-DataAnalyst/
│
├── retail_sales_eda.ipynb   # EDA notebook
├── retail_sales.csv         # Dataset (if included)
└── README.md                # Project documentation
```

*Note: Update the filenames above to match your actual project files.*

## Analysis Performed

### 1. Data Loading and Initial Inspection

- Load the retail sales dataset.
- Examine the number of rows and columns.
- Check column data types.
- Identify missing values and potential data quality issues.

### 2. Descriptive Statistics

Calculate the following statistical measures for numerical columns:

- Mean
- Median
- Mode
- Standard deviation

These statistics help summarize the dataset and understand the distribution of numerical variables.

### 3. Time Series Analysis

- Analyze monthly sales trends using line charts.
- Calculate and visualize quarterly sales performance.
- Identify sales fluctuations, growth patterns, and potential seasonal trends.

### 4. Customer Demographics Analysis

- Analyze the distribution of customer age groups.
- Examine the gender breakdown of customers.
- Explore purchasing behaviour across customer segments where the available data supports it.

### 5. Product Performance Analysis

- Identify the top 10 best-selling products.
- Calculate total revenue by product category.
- Visualize category-wise revenue using bar charts.

### 6. Correlation Analysis

- Generate a correlation matrix for numerical variables.
- Create a heatmap using Seaborn.
- Examine relationships between variables while distinguishing correlation from causation.

### 7. Additional Exploratory Visualization

Create an additional visualization to uncover potentially non-obvious business insights, such as:

- Payment method preferences across regions.
- Revenue contribution by customer segment.
- Differences in average transaction value across categories.

The final visualization will depend on the columns available in the dataset.

## Key Findings and Business Insights

The notebook includes observations after each visualization to explain the patterns revealed by the data.

The final findings focus on:

- Monthly and quarterly sales performance.
- Customer demographic patterns.
- Best-selling products and high-revenue categories.
- Relationships between numerical variables.
- Additional customer purchasing or payment trends.

**Note:** Specific findings should be documented after completing the analysis and validating the results against the dataset.

## Business Recommendations

Based on the findings, the analysis aims to develop actionable recommendations such as:

1. **Inventory Optimization:** Maintain sufficient stock of consistently best-selling products and monitor slow-moving items to reduce inventory costs.

2. **Targeted Marketing:** Design customer campaigns around demographic segments and purchasing patterns supported by the analysis.

3. **Sales Planning:** Use monthly and quarterly sales trends to improve demand forecasting, promotional timing, and inventory planning.

4. **Product Category Strategy:** Evaluate high-revenue categories when allocating marketing budgets and planning product promotions.

5. **Customer Experience:** Use observed regional payment preferences to prioritize convenient payment options for customers.

These recommendations should be refined using the actual analysis results rather than assumed trends.

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/avinashchetry-cloud/Oasis-Infobyte-DataAnalyst.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Oasis-Infobyte-DataAnalyst
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open the EDA notebook and run the cells sequentially.

Ensure that the dataset is available at the file path specified in the notebook.

## Conclusion

This project demonstrates the application of exploratory data analysis to transform raw retail sales data into meaningful insights. By combining statistical summaries, time series analysis, customer demographics, product performance analysis, and visualizations, the project provides a foundation for informed retail business decisions.

## Author

**Avinash Chetry**

Data Analyst Intern — Oasis Infobyte

GitHub: [avinashchetry-cloud](https://github.com/avinashchetry-cloud)

---

*Task 1: Exploratory Data Analysis on Retail Sales Data | Oasis Infobyte Internship*
