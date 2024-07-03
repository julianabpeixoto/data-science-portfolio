# Exploratory Data Analysis of Online Sales

## Project Overview
This project, the final project of Module 2: Programming Techniques I (Python) of 'Santander Coders 2023 | 2nd Semester—DS (3)', taught by Thiago Tavares Magalhães and Aruã de Mello Sousa, is a hands-on exploration of real-world online sales data. It offers a unique opportunity to apply theoretical knowledge to practical scenarios.

### Specific Objectives
Extract insights and better understand the phenomenon of sales and its related aspects:
- Customers
- Suppliers
- Products
- Payments
- Etc.

Throughout this project, I applied the knowledge I learned about Numpy, Pandas, and Git during the module to gain a deeper understanding of the data and draw meaningful insights.

### Tasks Completed:
1. **Data Loading and Initial Inspection**:
   - Read datasets into Pandas DataFrame objects and performed initial inspections to understand the structure and content of the data. This included examining the number of records, column names, and data types and identifying missing values.

2. **Exploratory Data Analysis (EDA)**:
   - Conducted an exploratory analysis to uncover patterns and insights within the data. This involved calculating statistical measures such as median, mean, minimum, maximum, and standard deviation for numerical columns and understanding the distribution of categorical column values.

3. **Answering Key Questions with Boolean Masking**:
   - Leveraged boolean masking and filtering techniques to answer specific questions about the data:
     - Which states have an order number above the average number of orders per state?
     - Which and how many cities with an order number greater than or equal to the median of towns with an average number of orders greater than or equal to the average per city belong to states with an order number greater than or equal to the average number of orders per state?
     - How many orders were delivered to the customer in 2016 or 2018?

4. **Data Manipulation and Feature Engineering**:
   - Created new features by generating ndarrays and adding them as new columns to the existing DataFrames. This involved deriving useful information from existing columns to enhance the dataset.

5. **Demonstrating Git Proficiency**:
   - Managed the project using Git, demonstrating version control skills by committing changes, branching, and collaborating effectively.

## About the Dataset

The Brazilian E-Commerce Public Dataset by Olist is available on [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) and comprises 9 .csv datasets. It is a public dataset under the [CC BY-NC-SA 4.0 license](https://creativecommons.org/licenses/by-nc-sa/4.0/) and is not updatable.

This dataset contains factual and anonymized information about 100,000 orders between 2016 and 2018 in various Brazilian marketplaces through the Olist Store. According to the description on Kaggle, its features allow visualizing an order under multiple dimensions:
- Order Status
- Price
- Payment and freight performance to the customer's location
- Customer reviews

A geolocation dataset also relates Brazilian postal codes to latitude and longitude coordinates.

From the provided data schema (available at this [link](https://i.imgur.com/HRhd2Y0.png), I initially opted to group the datasets, in a very simplified way, into two informational sets:

### Information on Actions Performed:
- Place order (orders_dataset.csv, order_items_dataset.csv)
- Pay (order_payments_dataset.csv)
- Receive payment (order_payments_dataset.csv)
- Receive the order (orders_dataset.csv)
- Review (order_reviews_dataset.csv)

### Information on the 'Actors' Involved in the Actions:
- Customers (customers_dataset.csv, geolocation_dataset.csv)
- Sellers (sellers_dataset.csv)
- Products (products_dataset.csv, product_category_name_translation.csv)

### Relevant Information about the Datasets:
- An order can have more than one product.
- Different sellers can sell products within the same order.
- The names of major Game of Thrones houses have replaced all references to companies and partners.
- Each order has a different customer ID (`customer_id`), and each customer has a unique general ID (`customer_unique_id`).

## References Used 

- Community and Module Content: Ada
- Alura: Articles on Numpy and Pandas
- [Numpy Documentation](https://pandas.pydata.org/docs/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)

## Main Skills and Features Used

- **Libraries**: Pandas, Numpy
- **Data Loading and Inspection**:
  - Loading datasets with Pandas
  - Inspecting data types, column names, and missing values
- **Exploratory Data Analysis (EDA)**:
  - Statistical summary of numerical columns (mean, median, min, max, standard deviation)
  - Proportion of categorical column values
- **Boolean Masking and Filtering**:
  - Filtering data to answer specific questions
- **Data Manipulation**:
  - Creating new columns using ndarrays
- **Version Control**:
  - Demonstrating Git proficiency

## Files

- **Data**: Contains the raw dataset files.
  - [Customers](olist_customers_dataset.csv)
  - [Geolocation](olist_geolocation_dataset.csv)
  - [Orders](olist_orders_dataset.csv)
  - [Order Items](olist_order_items_dataset.csv)
  - [Order Payments](olist_order_payments_dataset.csv)
  - [Order Reviews](olist_order_reviews_dataset.csv)
  - [Products](olist_products_dataset.csv)
  - [Product Category Translation](product_category_name_translation.csv)
  - [Sellers](olist_sellers_dataset.csv)
 
- **Code**: Contains the Python script used for the analysis and the detailed report on the analysis and findings.
  - [Code](jbp_projeto_final.ipynb)
 
- **Output**: Contains the terminal output with the git commands used during the project
   - [Terminal outputs](jbp_projeto_final_terminal_outpu.txt)

## Contact

Feel free to contact me with any questions or want to collaborate on future projects.

- **Email**: (jbertolucci@gmail.com)
- **LinkedIn**: (https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: (https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!

---
