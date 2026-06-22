# Advanced Exploratory Data Analysis on E-Commerce Dataset Using Python
Advanced Exploratory Data Analysis (EDA) project on an E-commerce dataset using Python, featuring data understanding, feature engineering, business-driven analysis, data manipulation, visualization, and correlation analysis.

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on an E-commerce dataset using Python.

The objective of this analysis is to understand customer purchasing behavior, identify sales patterns, discover revenue opportunities, and generate business insights through various data manipulation and visualization techniques.

The project covers the complete EDA workflow, including:

- Data Understanding
- Feature Engineering
- Data Manipulation
- Group By Analysis
- Sorting and Filtering
- Datetime Analysis
- Pivot Tables
- Crosstab Analysis
- Correlation Analysis
- Business Insights Extraction

---

## Tools and Libraries

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Dataset Information
Dataset: ecommerce

Source:
(ecommerce.csv)

The dataset contains E-commerce transaction records including:

- Invoice Number
- Product Description
- Quantity Purchased
- Unit Price
- Customer Information
- Country
- Transaction Date

---

# Data Understanding

Several exploratory steps were performed:

### Dataset Inspection

- Shape Analysis
- Data Type Inspection
- Descriptive Statistics
- Missing Value Check
- Duplicate Check

### Feature Engineering

New features were created to support business analysis:

| Feature | Description |
|----------|-------------|
| Revenue | Quantity × UnitPrice |
| Year | Transaction Year |
| Month | Transaction Month |
| Month_Name | Transaction Month Name |
| Day | Transaction Day |

---

# Business Questions and Analysis

## Question 1

### Which country generates the highest revenue?

Method Used:

- Group By
- Aggregation
- Sorting

Visualization:

![Top 10 Revenue by Country](Ecommerce%20Analysis/Top%2010%20Revenue%20by%20Country.png)

### Key Insight

United Kingdom contributes the largest revenue and can be considered the company's primary market.

---

## Question 2

### Which products have the highest sales quantity?

Method Used:

- Group By
- Sorting

Visualization:

![Top Selling Products](Ecommerce%20Analysis/Top%20Selling%20Products.png)

### Key Insight

Several products dominate total sales volume and should become a focus for inventory planning.

---

## Question 3

### How does revenue change across months?

Method Used:

- Datetime Analysis
- Group By Aggregation

Visualization:

![Monthly Revenue Trend](Ecommerce%20Analysis/Monthly%20Revenue%20Trend.png)

### Key Insight

Revenue generally increased throughout the year and reached its peak in November, indicating strong year-end sales activity.

---

## Question 4

### How does revenue vary across countries and months?

Method Used:

- Pivot Table
- Heatmap Visualization

Visualization:

![Revenue by Country and Month](Ecommerce%20Analysis/Revenue%20by%20Country%20and%20Month%20(Pivot%20Table).png)

### Key Insight

The United Kingdom dominates revenue generation across almost all months, highlighting a strong market dependency.

---

## Question 5

### Which countries have the highest number of transactions?

Method Used:

- Crosstab
- Heatmap Visualization

Visualization:

![Customer Purchasing Behavior](Ecommerce%20Analysis/Customer%20Purchasing%20Behavior%20(Crosstab).png)

### Key Insight

Most transactions belong to the low-price category, while premium products contribute only a small portion of total transactions.

---

# Correlation Analysis

## Correlation Heatmap

Visualization:

![Correlation Heatmap](Ecommerce%20Analysis/Correlation%20Heatmap.png)

### Insight

- Quantity has a strong positive correlation with Revenue (0.79).
- UnitPrice has a weak relationship with Revenue (0.09).
- Revenue growth is primarily driven by sales volume rather than product price.

---

# Key Findings

1. United Kingdom is the largest contributor to company revenue.
2. Revenue shows an increasing trend toward the end of the year.
3. Product sales are concentrated on a small number of high-performing products.
4. Most transactions occur within low-price product categories.
5. Sales volume has a stronger impact on revenue than product pricing.
6. The business is highly dependent on the United Kingdom market.

---

# Conclusion

This EDA project demonstrates how data manipulation techniques such as filtering, sorting, grouping, pivot tables, crosstabs, datetime analysis, and correlation analysis can be used to transform raw transaction data into actionable business insights.

The findings can support decision-making related to marketing strategy, inventory management, customer behavior analysis, and revenue optimization.
