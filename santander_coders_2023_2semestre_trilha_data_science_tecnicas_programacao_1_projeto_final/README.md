# Exploratory Data Analysis of Online Sales

## Project Overview
This project, the final project of Module 2: Programming Techniques I (Python) of 'Santander Coders 2023 | 2º Semestre—DS (3)', taught by Thiago Tavares Magalhães and Aruã de Mello Sousa, is a hands-on exploration of real-world online sales data. It offers a unique opportunity to apply theoretical knowledge to practical scenarios.

### Specific Objectives
Extract insights and better understand the phenomenon of sales and its related aspects:
- Customers
- Suppliers
- Products
- Payments
- Etc.

Throughout this project, I will apply the knowledge learned about Numpy, Pandas, and Git during the module.

### Tasks to Complete:
1. Read at least two datasets (.csv) as Pandas DataFrame objects and work with these DataFrame objects.
2. Perform an initial exploratory analysis of the tables:
   - Number of records
   - Column names and data types
   - Number of missing data (nulls or NaN)
   - Proportion of each value for categorical columns
   - For each numerical column, calculate statistical measures such as:
     - Median
     - Mean
     - Minimum
     - Maximum
     - Standard deviation
3. Raise and answer at least three questions about the data requiring a filter by boolean selection mask. The questions used in the analysis were:
   - Which states have an order number above the average number of orders per state?
- Which and how many cities with an order number greater than or equal to the median of towns with an average number of orders greater than or equal to the average per city belong to states with an order number greater than or equal to the average number of orders per state?
- How many orders were delivered to the customer in 2016 or 2018 (order_delivered_customer_date)?
4. At least twice, create an ndarray and add it to a table as a new column.
   - For this, I was asked to find some helpful information that can be derived from the columns already existing in the table.
5. Demonstrate knowledge of GIT.

## About the Dataset

The Brazilian E-Commerce Public Dataset by Olist is available on Kaggle and composed of 9 .csv datasets. It is a public dataset under the CC BY-NC-SA 4.0 license and is not updatable.

This dataset contains factual and anonymized information about 100,000 orders between 2016 and 2018 in various Brazilian marketplaces through the Olist Store. According to the description on Kaggle, its features allow visualizing an order under multiple dimensions:
- Order Status
- Price
- Payment and freight performance to the customer's location
- Customer reviews

A geolocation dataset also relates Brazilian postal codes to latitude and longitude coordinates.

From the provided data schema (available at this link), I initially opted to group the datasets, in a very simplified way, into 2 informational sets:
Information on Actions Performed:
Place order (orders_dataset.csv, order_items_dataset.csv)
Pay (order_payments_dataset.csv)
Receive payment (order_payments_dataset.csv)
Receive the order (orders_dataset.csv)
Review (order_reviews_dataset.csv)
Information on the 'Actors' Involved in the Actions:
Customers (customers_dataset.csv, geolocation_dataset.csv)
Sellers (sellers_dataset.csv)
Products (products_dataset.csv, product_category_name_translation.csv)

### Relevant Information about the Datasets:
- An order can have more than one product.
- Different sellers can sell products within the same order.
- The names of major Game of Thrones houses have replaced all references to companies and partners.
- Each order has a different customer ID (`customer_id`), and each customer has a unique general ID (`customer_unique_id`).

## References Used in This Project
- Community and Module Content: Ada
- Alura: Articles on Numpy and Pandas
- Numpy Documentation
- Pandas Documentation
