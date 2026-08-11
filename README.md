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
- **Final Columns:** 24 after feature engineering
- **Added Features:** `Year`, `CustomerKey`, `BrandTotalAmount`, `OrderShippingCost`
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
| `Year` | Year extracted from `OrderDate` |
| `CustomerKey` | Customer-level key created from `CustomerID` and `CustomerName` |
| `BrandTotalAmount` | Total sales amount associated with each brand |
| `OrderShippingCost` | Shipping cost associated with each order |

### Data Quality

- No missing values were found.
- No duplicate rows were found.
- `OrderDate` was converted to datetime.
- `Year` was extracted from `OrderDate`.
- `CustomerKey` was created because `CustomerID` was not always sufficient as a unique customer identifier.
- `BrandTotalAmount` was created to analyze total sales performance by brand.
- `OrderShippingCost` was created to analyze shipping cost at the order level.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
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
