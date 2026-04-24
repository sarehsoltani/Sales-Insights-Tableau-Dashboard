# Tableau Sales Analytics Pipeline

![Dashboard Preview](Tableau Dashboard.png)

## Project Overview
This project provides detailed business intelligence insights into the sales of a branch shop operating across multiple markets. The insights are derived from a sales database containing customer information, transaction records, market names, and product details.

By bridging a **MySQL** database with **Tableau**, this project demonstrates a full end-to-end data pipeline—from raw SQL data to a polished, interactive dashboard used for executive decision-making.

## Tools & Technologies Used
* **Tableau Desktop:** Primary tool for data visualization and dashboard design.
* **MySQL & MySQL Workbench:** RDBMS used to store, manage, and query sales records.
* **SQL:** Used for data discovery and complex transformations.
* **MySQL JDBC Connector:** Established the live bridge between the database and the BI layer.

## Data Modeling & ETL Process
This project follows a structured **ETL (Extract, Transform, Load)** workflow to ensure data integrity and performance:

1.  **Extraction:** Pulled raw transactional data from a MySQL relational database.
2.  **Data Modeling (Star Schema):** Designed a high-performance schema connecting a Central Fact Table (`Transactions`) to multiple Dimension Tables (`Customers`, `Markets`, `Products`, and `Date`) using primary and foreign key relationships.
3.  **Transformation:** * Performed data cleaning via SQL to remove invalid entries.
    * Implemented **Currency Normalization** through custom Tableau calculated fields to standardize revenue across USD and INR transactions.
4.  **Loading:** Structured the final dataset into Tableau for real-time interactive analysis.



## 🚀 Key Features & Functionality
* **Interactive Filtering:** Global year-over-year (2017–2020) toggles.
* **KPI Tiles (BANs):** Dynamic summaries of Total Revenue and Sales Quantity.
* **Regional & Customer Analysis:** Identification of top-performing markets (Delhi NCR) and key customer segments.
* **Temporal Trends:** Monthly revenue tracking to identify seasonal sales cycles.

