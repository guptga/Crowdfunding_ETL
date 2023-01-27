# Crowdfunding_ETL

### Overview

1) Extracting and transforming the data from a large Excel files into CSV files.

2) Creating a PostgreSQL database and tables by using an ERD.

3) Loading the CSV files into the SQL database.

4) Performing SQL queries to generate reports for stakeholders.

### Aim

The aim of this project is to build a database with SQL. This way, analysis can be performed and reports can be created for company stakeholders.

Resources

Data Source: crowdfunding.xlsx - contacts.csv
Software: Jupyter Notebook, PostgreSQL, pgAdmin 4


### Analysis of Data and Results

The ETL process f is divided into the following steps:

Step 1: Extract the Data

Using Python and Pandas we have extracted:

4 CSV files are extracted from crowdfunding.xlsx file and contacts.xlsx using the code 

To extract these CSV files 2 methods were used:

Python dictionary method.
Regular expression method.
Step 2: Transform and Clean Data
Using Python, Pandas, and data cleaning strategies, we have transformed the data via formatting, splitting, converting data types, and restructuring to create DataFrames that can be loaded into a postgreSQL database as a CSV file.

When finishing this step, we have 5 CSV cleaned files saved as:

contacts.csv
category.csv
subcategory.csv
capaign.csv
backers.csv
Codes used in this step is also saved as Extract-Transform_starter_code.ipynb (https://github.com/MireyNM/Crowdfunding-ETL/blob/main/Extract-Transform_final_code.ipynb)

Step 3: Create an ERD and Table Schema, and Load Data
In order to load the cleaned datasets as CSV files into an SQL database we started by creating an Entity Relationship Diagram (ERD) using Quick DBD website (https://www.quickdatabasediagrams.com/).

When the database schema is complete, we have saved the ERD as crowdfunding_db_relationships.png (See Fig.1) and we have saved the database schema as a PostgreSQL file named crowdfunding_db_schema.sql (https://github.com/MireyNM/Crowdfunding-ETL/blob/main/crowdfunding_db_schema.sql)

Outcomes_vs_Goals

Figure 1 - Crowfunding Entity Relationship Diagram (ERD)

The next step was to pass and run the PostgreSQL file into PgAdmin query editor in order to create the tables. Finally, we have uploaded the CSV cleaned files into these tables.
