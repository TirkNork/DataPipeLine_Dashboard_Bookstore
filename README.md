# Data Pipeline for Dynamic Dashboard of Bookstore

The objective of this project was to develop an ETL (Extract, Transform, Load) pipeline for acquiring bookstore data from MySQL databases and APIs,
then storing it in GCP (Google Cloud Platform) cloud storage. The data processing was conducted using pandas, while the workflow was orchestrated
using Apache Airflow. Subsequently, the transformed data was loaded into GCP BigQuery for further analysis.

In addition, Looker Studio was leveraged to craft dynamic dashboards tailored for analyzing revenue, top-selling categories, and other data related to the bookstore. 
These dashboards were equipped with search and filtering functionalities to enhance data exploration and decision-making processes.

[This project is part of Online course: Road to Data Engineer 2.0]

![Alt text](img/overview.png?raw=true "Title")

## Example Data
- Raw data
  - Customer data: Information about each customer
  - Transaction data: Transaction in bookstore
  - Conversion_rata API: API for call conversion_rate of dollar and Thai baht in each day
    
![Alt text](img/ex_data.png?raw=true "Title")

- Transformed data -> Merge Customer data and Transaction data, calculate price in Thai Baht with conversion rate, Transform data format in some column.


![Alt text](img/transformed_data.png?raw=true "Title")

## Dashboard

The Bookstore dynamic dashboard developed by Looker Studio comprises two pages, The first page provides an overview of various metrics including Total Revenue,
Total Customers, Revenue by Country, Transaction by Country, Best Selling Books, Best Selling Categories, each dashboard can filter with Country and Month Year.

![Alt text](img/dash1.png?raw=true "Title")

The second page is dedicated to creating a table displaying Book titles and Revenue, filtered by Revenue. This dashboard aims to identify which books should be prioritized for promotion based on their revenue performance.

![Alt text](img/dash2.png?raw=true "Title")



Dashboard link: https://lookerstudio.google.com/reporting/f90d5ab5-ad04-494b-acf4-6c76bfaa110e




