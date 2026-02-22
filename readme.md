# **🛒 Online Retail Customer Segmentation & Retention Analysis**

## 📌 Project Objective

The goal of this project is to analyze transaction-level retail data to:
- Understand customer purchasing behavior
- Segment customers using RFM analysis
- Identify potentially inactive (churn-risk) customers
- Provide data-driven retention strategies
This project simulates real-world business analytics in an e-commerce environment.

## 📊 Dataset Overview

The dataset contains transaction-level records from an online retail company.
Each row represents:
A single product line item within an invoice (not a full order or customer).

Key columns:

- InvoiceNo — Order ID
- StockCode — Product ID
- Quantity — Units purchased
- UnitPrice — Price per unit
- InvoiceDate — Purchase timestamp
- CustomerID — Unique customer identifier
- Country — Customer location

**🧹 Step 1: Data Understanding & Cleaning**

The following preprocessing steps were performed:

✔ Removed rows with missing CustomerID

✔ Removed cancelled invoices (InvoiceNo starting with "C")

✔ Removed invalid transactions (Quantity ≤ 0 or UnitPrice ≤ 0)

✔ Converted InvoiceDate to datetime format

✔ Created a Revenue column (Quantity × UnitPrice)

After cleaning, the dataset contains only valid completed purchases suitable for customer-level analysis.