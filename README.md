# Amazon Sales Analysis

## Project Overview

This project analyzes an Amazon Sales dataset to understand order patterns, customer behavior, product performance, seller performance, and geographic sales distribution.

The goal is to turn raw sales data into clear business insights that can support better decisions related to products, marketing, customers, inventory, and markets.

## Problem Statement

The business has a large amount of sales and order data, but raw data alone does not clearly show which products, categories, brands, customers, sellers, and markets are performing best.

This project aims to identify the main sales patterns and translate them into actionable business insights.

## Objectives

- Analyze overall sales and order performance.
- Understand customer purchasing behavior and repeat purchases.
- Identify the best and weakest products.
- Compare category and brand performance.
- Analyze sales across countries and states.
- Compare seller performance.
- Explore order value, quantity, and shipping cost.
- Extract actionable business insights.
- Provide recommendations based on the analysis.

## Dataset

### Dataset Source

The project uses an **Amazon Sales Dataset**.

**Original Dataset:** [Amazon Sales Dataset on Kaggle](https://www.kaggle.com/)

> The provided notebook does not contain a dataset-specific Kaggle URL, so the link above points to the Kaggle source rather than an unverified specific dataset page.

### Dataset Size

- **Rows:** 100,000
- **Original Columns:** 20
- **Final Columns:** 22 after feature engineering
- **Time Period:** 2020–2024

### Important Features

| Feature | Description |
|---|---|
| `OrderID` | Order identifier |
| `OrderDate` | Order date |
| `CustomerID` | Customer identifier |
| `CustomerName` | Customer name |
| `ProductID` | Product identifier |
| `ProductName` | Product name |
| `Category` | Product category |
| `Brand` | Product brand |
| `Quantity` | Number of units ordered |
| `UnitPrice` | Price per unit |
| `Discount` | Applied discount |
| `Tax` | Order tax |
| `ShippingCost` | Shipping cost |
| `TotalAmount` | Total order amount |
| `PaymentMethod` | Payment method |
| `OrderStatus` | Order status |
| `City` | Customer city |
| `State` | Customer state |
| `Country` | Customer country |
| `SellerID` | Seller identifier |
| `Year` | Extracted order year |
| `CustomerKey` | Customer-level key created from CustomerID and CustomerName |

### Data Quality

- No missing values were found.
- No duplicate rows were found.
- `OrderDate` was converted to datetime.
- `Year` was extracted from `OrderDate`.
- `CustomerKey` was created because `CustomerID` was not always sufficient as a unique customer identifier.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Workflow

```text
Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Data Transformation
      ↓
Exploratory Data Analysis
      ↓
Data Visualization
      ↓
Insights
      ↓
Recommendations
```

## Key Insights

### Best Performers

- **Best Product:** LED Desk Lamp — **6,344 units** sold.
- **Best Category:** Electronics — **16,853 orders**.
- **Best Brand:** CoreTech — approximately **8.57M** in sales.
- **Best Market:** United States — **70,058 orders**.
- **Best State:** Texas — **24,896 orders**.
- **Highest Year:** 2023 — **20,096 orders**.

### Areas to Improve

- **Lowest Product:** Children's Book — **5,619 units**.
- **Lowest Category:** Clothing — **16,439 orders**.
- **Lowest Brand:** HomeEase — approximately **8.30M** in sales.
- **Lowest Market:** Australia — **4,130 orders**.
- **Customer Behavior:** Most customers made only **1 order**, making customer retention an important opportunity.
- **Order Value:** Average order value is approximately **918**, while the median is approximately **714**.

## Recommendations

1. **Focus on high-performing products**  
   Prioritize products with strong demand, especially LED Desk Lamp.

2. **Invest in strong categories and brands**  
   Maintain strong inventory and marketing for Electronics and CoreTech products.

3. **Focus on key markets**  
   Prioritize the United States, especially Texas, when allocating marketing and inventory resources.

4. **Improve customer retention**  
   Use loyalty programs, personalized offers, and follow-up campaigns to encourage one-time customers to purchase again.

5. **Improve weaker areas**  
   Review lower-performing categories, brands, products, and markets to identify opportunities for better pricing, promotions, or product selection.

6. **Compare seller performance**  
   Analyze top and low-performing sellers to identify successful products and selling strategies.

## Conclusion

The analysis shows that sales performance varies across products, categories, brands, customers, sellers, and geographic markets.

Electronics, CoreTech, the United States, and Texas are among the strongest areas, while most customers make only one purchase. Maintaining strong-performing areas while improving customer retention and weaker markets can provide opportunities for future growth.
