# Data Warehouse Project

This repository contains the submission for the Data Warehouse project, part of the Virtual Internship Experience for Data Engineer Test at ID/X Partners.
Canva PPT : https://www.canva.com/design/DAFkcoRmS_k/78Ly8ptRvkJ-KdBotZ8wHA/edit?utm_content=DAFkcoRmS_k&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton 
## Introduction

The project involves creating a Data Warehouse for an e-commerce client of ID/X Partners, comprising a Fact table and several Dimension tables derived from the source database.

## Tasks

1. **Import/Restore Database Staging**
   - Execute `scripts/import_staging.sql` to import/restore the Staging database.

2. **Database and Table Creation**
   - Create a database named DWH_Project.
   - Create Fact and Dimension tables based on the tables in the Staging database using `scripts/create_tables.sql`.

3. **Talend ETL Job**
   - Develop a Talend ETL job in `talend/etl_job.talend` to transfer data from Staging to Data Warehouse.
   - Implement data transformation for `DimCustomer`: Convert FirstName and LastName to uppercase and combine into a new column, CustomerName.

4. **Summary Sales Order Procedure**
   - Implement a Stored Procedure (SP) in `stored_procedures/summary_sales_order.sql` to display a summary of sales orders based on delivery status.

## Setup

1. Run `scripts/import_staging.sql`.
2. Execute `scripts/create_tables.sql`.
3. Open and execute the Talend ETL job in `talend/etl_job.talend`.
4. Execute `stored_procedures/summary_sales_order.sql` to create the Summary Sales Order Stored Procedure.

## ETL Process

Describe the ETL process and flow of data from Staging to Data Warehouse. Include specific configurations made in the Talend ETL job.

## Transformations

Explain the data transformation applied to the `DimCustomer` table, especially the conversion of FirstName and LastName to uppercase and the creation of the new column `CustomerName`.

## Summary Sales Order Procedure

Detail the implementation of the Summary Sales Order Stored Procedure, including input parameters and logic used for summarizing sales orders based on delivery status.

