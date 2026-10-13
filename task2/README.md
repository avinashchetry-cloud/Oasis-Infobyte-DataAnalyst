# E-Commerce Customer Segmentation using K-Means Clustering

## Project Overview

This project focuses on segmenting an e-commerce company's customer base based on purchasing behaviour using the K-Means clustering algorithm. The goal is to identify distinct customer groups and provide actionable insights that can help businesses develop targeted marketing strategies, improve customer retention, and identify high-value customers.

The project uses Recency, Frequency, and Monetary (RFM) analysis to create behavioural features for customer segmentation.

## Objectives

- Perform exploratory data analysis on e-commerce transaction data.
- Inspect the dataset and handle missing or inconsistent values.
- Calculate customer-level Recency, Frequency, and Monetary values.
- Standardize behavioural features using `StandardScaler`.
- Determine the optimal number of clusters using the Elbow Method.
- Apply K-Means clustering to segment customers.
- Visualize customer clusters and compare their purchasing behaviour.
- Profile each cluster and recommend suitable marketing strategies.

## Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment:** Jupyter Notebook
- **Algorithm:** K-Means Clustering
- **Dataset:** Online Retail Dataset from the UCI Machine Learning Repository

## Dataset

The project uses the Online Retail dataset, which contains transactional data from a UK-based online retail business.

Important columns include:

| Column | Description |
|---|---|
| `Invoice` | Invoice or transaction identifier |
| `StockCode` | Product identifier |
| `Description` | Product description |
| `Quantity` | Number of units purchased |
| `InvoiceDate` | Date and time of the transaction |
| `Price` | Unit price of the product |
| `Customer ID` | Customer identifier |
| `Country` | Customer's country |

Dataset source: [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

## Project Workflow

### 1. Data Loading and Inspection

- Loaded the dataset using Pandas.
- Inspected the dataset structure, column types, and descriptive statistics.
- Checked for missing values and inconsistent transaction records.
- Examined negative quantities and cancelled invoices.

### 2. Exploratory Data Analysis

Performed descriptive analysis to understand transaction patterns and customer purchasing behaviour.

The analysis includes:
- Revenue calculation using quantity and unit price.
- Customer purchase frequency.
- Customer-level spending analysis.
- Inspection of unusual and negative transaction values.

### 3. RFM Feature Engineering

Created three customer-level behavioural features:

- **Recency:** Number of days since the customer's most recent purchase.
- **Frequency:** Number of unique invoices associated with the customer.
- **Monetary:** Total transaction value associated with the customer.

Revenue for each transaction line was calculated as:

`Revenue = Quantity × Price`

These features provide a customer-level representation of purchasing behaviour.

### 4. Feature Standardization

Applied `StandardScaler` to standardize the RFM features before clustering.

Standardization is important because Recency, Frequency, and Monetary values have different scales. Scaling prevents features with larger numerical values from disproportionately influencing distance calculations.

### 5. K-Means Clustering

Applied the K-Means clustering algorithm to group customers with similar purchasing behaviour.

The Elbow Method was used to compare inertia values across different numbers of clusters and identify a reasonable value of K.

### 6. Cluster Visualization

Visualizations were created to understand the clustering results and compare customer segments.

These include:
- Elbow plot for selecting the number of clusters.
- Scatter plots comparing different RFM feature combinations.
- Bar chart showing the number of customers in each cluster.
- Cluster profile table comparing average Recency, Frequency, and Monetary values.

### 7. Customer Segmentation

Cluster profiles were examined to interpret customer behaviour and assign descriptive labels.

The analysis identifies potential segments such as:

- **Average Customers:** Customers with moderate purchasing activity and spending.
- **Lapsed Customers:** Customers whose most recent purchases occurred relatively long ago.
- **Whale Customers:** Customers with exceptionally high purchasing frequency and monetary value.

These labels are based on observed cluster characteristics rather than predefined K-Means categories.

## Business Insights and Marketing Recommendations

| Customer Segment | Recommended Marketing Strategy |
|---|---|
| Average Customers | Encourage repeat purchases through loyalty rewards, personalized offers, and product recommendations. |
| Lapsed Customers | Use re-engagement campaigns, targeted discounts, and personalized reminders to encourage customers to return. |
| Whale Customers | Focus on customer retention through premium services, exclusive offers, loyalty benefits, and personalized experiences. |

The final marketing strategy should be guided by the actual RFM profiles and characteristics of each cluster.

## Key Learnings

- Performing exploratory data analysis on transactional datasets.
- Cleaning and preparing real-world customer data.
- Engineering customer-level RFM features using Pandas.
- Applying feature standardization before distance-based clustering.
- Using the Elbow Method to select a suitable number of clusters.
- Applying K-Means for unsupervised customer segmentation.
- Interpreting clusters and translating analytical findings into business recommendations.

## How to Run the Project

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
```

### 3. Download the Dataset

Download the Online Retail dataset from the UCI Machine Learning Repository and place the dataset file in the appropriate project directory.

### 4. Run the Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells sequentially.

## Conclusion

This project demonstrates how unsupervised machine learning can be used to identify customer segments from transactional data. By combining RFM analysis, standardization, K-Means clustering, and visualizations, businesses can better understand purchasing behaviour and develop more targeted customer engagement strategies.

The resulting customer segments provide a foundation for improving retention, recognizing high-value customers, and supporting data-driven marketing decisions.
