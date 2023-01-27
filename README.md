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

The ETL process is divided into the following steps:

**Step 1**: Extract the Data

Using Python and Pandas we have extracted:

  1) 4 CSV files from **crowdfunding.xlsx** file and **contacts.xlsx** using the code 

  2) To extract these CSV files either of the 2 methods were used and we chose the **Option 1 :** 


        **Option 1** - Python dictionary method.

        **Option 2** - Regular expression method.

**Step 2:** Transform and Clean Data

Using Python, Pandas, and data cleaning strategies, we have transformed the data via formatting, splitting, converting data types, and restructuring to create DataFrames that can be loaded into a postgreSQL database as a CSV file.

When finishing this step, we have 4 CSV cleaned files saved as:

contacts.csv

category.csv

subcategory.csv

campaign.csv


**Step 3:** Create an ERD and Table Schema, and Load Data


In order to load the cleaned datasets as CSV files into an SQL database we started by creating an Entity Relationship Diagram (ERD) using Quick DBD website (https://www.quickdatabasediagrams.com/).

    1) When the database schema is complete, we have saved the ERD as crowdfunding_db_schema.png and we have saved the database schema as a PostgreSQL file named crowdfunding_db_schema.sql

![crowdfunding_db_schema](https://user-images.githubusercontent.com/116124534/214982917-58198bd4-b327-4fd8-a634-d2fcdca4f647.png)



The next step was to pass and run the PostgreSQL file into PgAdmin query editor in order to create the tables. Finally, we have uploaded the CSV cleaned files into these tables.
