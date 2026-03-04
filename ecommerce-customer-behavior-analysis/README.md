📊 E-commerce Customer Behavior Analysis
📌 Project Overview

This project performs an Exploratory Data Analysis (EDA) on an e-commerce transactions dataset to understand customer behavior, revenue distribution, product performance, and seasonality.
The goal is to derive business-relevant insights from raw transactional data.

🎯 Objectives

Understand the structure and quality of the data

Identify and handle returns and cancellations

Analyze revenue across countries and products

Study monthly revenue trends and seasonality

📂 Dataset

Source: Online Retail Dataset (UCI / Kaggle)

Records: ~1 million transactions

Time Period: 2009 – 2011

Key Fields: Invoice, Product, Quantity, Price, Customer ID, Country, Invoice Date

🧹 Data Cleaning & Preparation

Key steps performed:

Converted InvoiceDate to datetime format

Identified credit notes (Invoice starting with “C”) as returns

Validated hypothesis using quantity and price distributions

Separated data into:

Sales transactions (positive quantity & price)

Returns / cancellations

Created a new Revenue feature (Quantity × Price)

📈 Key Insights
🌍 Country-wise Revenue

The United Kingdom dominates revenue, contributing the majority of total sales

Other significant markets include EIRE, Netherlands, Germany, and France

Business is highly UK-centric

📦 Product Performance

Revenue is highly concentrated among a small number of products

A few top products contribute disproportionately to total revenue

Non-product charges (e.g., postage) also form a noticeable share of revenue

📅 Monthly Revenue Trend

Clear seasonal pattern observed

Revenue increases from August, peaks during October–November

Sharp decline post-November, indicating post-holiday slowdown

🧠 Business Interpretation

Strong dependence on seasonal (Q4) demand suggests inventory and marketing focus should be highest during this period

Returns should be analyzed separately to understand product or fulfillment issues

Growth opportunities exist in non-UK markets, though current contribution is limited

🛠️ Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn

Jupyter Notebook

✅ Conclusion

This analysis demonstrates a structured, hypothesis-driven EDA approach using real-world data.
It highlights how data cleaning, validation, and aggregation can translate raw transactions into actionable business insights.