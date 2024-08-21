# Crowdfunding_ETL
Project #2
ETL Mini Project

Overview

This project is a demonstration of the ETL (Extract, Transform, Load) process applied to a set of data related to crowdfunding campaigns. The primary goal of this project is to extract data from various sources, transform it to meet specific criteria, and then load it into a structured format suitable for analysis.

Project Objectives

Extract data from multiple sources.
Transform the data to ensure it is clean, organized, and ready for analysis.
Load the transformed data into a final format that can be used for further data analysis or reporting.

Data Sources

The following data was provided by the class:

crowdfunding.xlsx: Contains details about crowdfunding campaigns, including campaign IDs, contact information, pledge amounts, and more.
contacts.xlsx: Includes contact information for the campaign organizers.

Project Structure

ETL_Mini_Project_RWillet_NRaver-Goldsby.ipynb: The main Jupyter notebook containing the ETL pipeline, code execution, and results.
Resources/: A directory containing the source data files and output files. 
The source files include crowdfunding.xlsx and contacts.xlsx
The ETL_Mini_Project_RWillet_NRaver-Goldsby.ipynb should return the following output files:  campaign.csv, category.csv, contacts.csv, and subcategory.csv 
We used quickdatabasediagrams.com to create and ERD which we then were able to export into Postgresql, to create the tables and relationships.
We then were able to upload the csv outputs into the Postgresql tables.

ETL Process

1. Extract
Data extraction is performed using Python's pandas library, which reads data from the provided Excel files. The data is imported into pandas DataFrames for further processing.

2. Transform
The transformation process includes:

Manipulating data creating several new columns including first and last names, category, and subcategory columns within our data frame.
Additionally, we drop repetetive columns. Then using our created columns we merge combining different data sources into a merged campaign dataframe.
Also, we used pandas to create a contacts dataframe from an excel sheet.
We converted dataframes into .csv files.


3. Load
The final, transformed data is loaded into a structured DataFrame. This DataFrame can then be exported to a CSV file or stored in a database for further use.

Results

The ETL process results in a cleaned and organized dataset, which is saved in the following formats:

campaign.csv, category.csv, contacts.csv, and subcategory.csv 

Theses results can also be uploaded into Postgresql for further manipulation.

How to Run the Project

Prerequisites
Ensure you have the following Python packages installed:

pandas
numpy
openpyxl (for working with Excel files)
json
datetime

After prerequisites, run the ETL_Mini_Project_RWillet_NRaver-Goldsby.ipynb in Jupyter notebook or VS code.

Project Assistance:

Use of learning assistant AI through Vanderbilt University resources.
We also recieved feedback from Gulseevi Rees throughout the project.

Authors:

Natalie Raver-Goldsby
Richard Willet




