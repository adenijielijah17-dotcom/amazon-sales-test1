# Amazon Sales Analysis using Pandas and SQL

## Project Overview
This project focuses on analyzing Amazon sales data to extract meaningful business insights.
The analysis is performed using **Pandas for data cleaning and preprocessing** and **SQL for
exploratory data analysis (EDA) and solving real-world business problems**.

The dataset contains product details, pricing, discounts, ratings, and customer reviews
from Amazon.

---

## Objectives
- Clean and preprocess Amazon sales data using Pandas
- Identify and handle missing values
- Perform exploratory data analysis using SQL queries
- Solve business-related questions based on sales and customer behavior
- Generate insights to support data-driven decision making

---

## Dataset Description
The dataset includes the following key attributes:
- Product ID and Product Name
- Category
- Discounted Price and Actual Price
- Discount Percentage
- Product Rating and Rating Count
- Customer Reviews and Review Metadata
- Product and Image Links

---

## Tools & Technologies
- **Python**
  - Pandas
  - NumPy
- **SQL**
  - MySQL / SQLite (for EDA queries)
- **VS Code**
- **Jupyter Notebook**

---

## Data Cleaning (Pandas)
The following data cleaning steps were performed using Pandas:
- Converted price and discount columns from string to numeric format
- Removed currency symbols and percentage signs
- Identified missing values across all columns
- Handled missing values in `rating_count`
- Ensured consistent data types for analysis

Example tasks:
- Missing value detection
- Data type conversion
- Data validation

---

## Missing Value Analysis
- The dataset contains missing values primarily in the `rating_count` column
- Missing values were analyzed and handled appropriately to avoid bias in analysis
- Other columns were verified to have no missing values

---

## Exploratory Data Analysis (SQL)
SQL was used to perform structured EDA and answer key analytical questions, such as:
- Category-wise average ratings
- Products with the highest discounts
- Top-rated products with significant review counts
- Relationship between discount percentage and customer ratings
- Price comparison across categories


---

## Business Problems Solved
This project addresses the following business questions:
- Which product categories offer the highest average discounts?
***sq
- select
category,
AVG(discounted_price) AS discount
from amazon
group by category
order by discount desc
limit 5;
***
- Do higher discounts lead to better customer ratings?
- Which products receive high ratings despite low discounts?
- What categories generate the most customer engagement based on rating count?
- How pricing strategies vary across different Amazon product categories

---

## Key Insights
- Certain categories consistently provide higher discounts
- High discounts do not always guarantee higher ratings
- Customer engagement varies significantly across product categories
- Some premium-priced products maintain strong ratings with minimal discounts

---

## Conclusion
This analysis demonstrates how combining **Pandas for data cleaning** and **SQL for EDA**
can effectively uncover actionable insights from e-commerce sales data.  
The project highlights the importance of data preprocessing and structured querying
to solve business problems in real-world datasets.

---

## Future Improvements
- Build interactive dashboards
- Perform sentiment analysis on customer reviews
- Apply machine learning models for sales prediction
- Automate data pipelines

---

## Author
Adeniji Elijah
# amazon-sales-test1
