# Retail-Sales-Customer-Segmentation

## Dataset Overview [Kaggle](https://www.kaggle.com/datasets/dataceo/sales-and-customer-data/data)
Sales Data: Contains transaction details such as invoice numbers, products purchased, quantities, prices, and shopping mall locations.
Customer Data: Provides demographic details like customer ID, gender, age, and payment method.

## Objectives
ETL Pipeline: Extract, transform, and load data from the sales and customer datasets.
Key Metrics: Analyze and report insights such as:
Total sales by category and shopping mall.
Customer segmentation by gender, age, and payment method.
Average purchase value by customer demographic.


## 1. Load the Data into MySQL
Create Tables
Define tables in MySQL to store sales and customer data:

** Sales Table
CREATE TABLE Sales (
    InvoiceNo VARCHAR(50),
    CustomerID INT,
    Category VARCHAR(100),
    Quantity INT,
    Price DECIMAL(10, 2),
    InvoiceDate DATE,
    ShoppingMall VARCHAR(100)
);

** Customers Table
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    Gender VARCHAR(10),
    Age INT,
    PaymentMethod VARCHAR(50)
);
