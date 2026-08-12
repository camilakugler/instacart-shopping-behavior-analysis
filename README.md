# Instacart Customer Shopping Behavior Analysis

## Overview

This project explores customer shopping behavior using a modified version of Instacart's public 2017 grocery-order dataset. The analysis focuses on cleaning and validating the data, identifying purchasing patterns, and communicating insights through exploratory data analysis and visualizations.

## Objective

The goal of the project is to understand how Instacart customers shop by analyzing:

- Order activity by hour of day and day of week
- Time between consecutive orders
- Number of orders per customer
- Typical number of items per order
- Most frequently purchased products
- Products most frequently reordered
- Reorder behavior across products

## Dataset

The project uses five related datasets:

- `instacart_orders.csv` — order-level information
- `order_products.csv` — products included in each order
- `products.csv` — product information
- `aisles.csv` — aisle categories
- `departments.csv` — department categories

The dataset used in this project is a modified subset of the original Instacart dataset, with missing and duplicated values included for data-cleaning practice.

Original public dataset:
- [Instacart — 3 Million Orders, Open Sourced](https://tech.instacart.com/3-million-instacart-orders-open-sourced-d40d29ead6f2)
- [Kaggle — Instacart Market Basket Analysis](https://www.kaggle.com/c/instacart-market-basket-analysis/overview)

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Analysis Workflow

1. **Data inspection** — reviewed dataset structure, data types, distributions, and relationships between tables.
2. **Data cleaning** — identified duplicate records and investigated missing values across the datasets.
3. **Data transformation** — merged related tables and prepared the data for analysis.
4. **Exploratory Data Analysis (EDA)** — analyzed shopping activity by time, customer, product, and order characteristics.
5. **Visualization** — created charts to communicate purchasing patterns and behavioral trends.

## Key Findings

- Order activity increases sharply in the morning and remains highest from approximately **9 AM to 4 PM**, before declining in the evening.
- Among the selected food-related departments analyzed, **Sunday showed the highest order volume**, with activity decreasing through the middle of the week and increasing again toward the weekend.
- Customer reorder intervals show clear recurring patterns, with **7-day and 30-day intervals** standing out in the distribution.
- The number of customers decreases as the number of orders per customer increases, indicating that lower order frequencies are more common in the analyzed sample.
- **Banana** was the most frequently purchased product, followed by **Bag of Organic Bananas, Organic Strawberries, Organic Baby Spinach, and Organic Hass Avocado**.
- Small and medium-sized baskets are the most common, with the number of orders declining substantially as basket size increases.
- Reordered-product rankings are also dominated by bananas, fruits, vegetables, and other organic products.

## Data Quality Findings

During preprocessing:

- Duplicate order records were identified and removed.
- Missing product names were concentrated in records assigned to an aisle and department labeled as missing.
- Missing cart-position values were associated with unusually large orders and were investigated before analysis.

## Repository Structure

```text
instacart-shopping-behavior-analysis/
│
├── README.md
├── instacart_analysis.ipynb
└── data/
    ├── instacart_orders.csv
    ├── order_products.csv
    ├── products.csv
    ├── aisles.csv
    └── departments.csv
```

> The dataset files may be omitted from the repository if they are too large or subject to distribution restrictions. In that case, include download instructions instead.

## Skills Demonstrated

`Python` `Pandas` `NumPy` `Data Cleaning` `EDA` `Data Visualization` `Data Wrangling` `Customer Behavior Analysis` `Reorder Analysis` `Jupyter Notebook`

## Conclusion

The analysis shows how transactional grocery data can be transformed into useful insights about customer shopping habits, purchase timing, basket composition, and product loyalty. The project demonstrates an end-to-end exploratory data analysis workflow, from data quality assessment and preprocessing to visualization and interpretation of customer behavior.
