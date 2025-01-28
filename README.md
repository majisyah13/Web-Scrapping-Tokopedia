# Web-Scrapping-Tokopedia

# Description
This project demonstrates the way to perform web scraping on an e-commerce website in Indonesia, specifically Tokopedia. 
Here, I provide an example of scraping data on "seblak" products listed on Tokopedia.

## A. Extract
The first stage in the data pipeline is `Extract`. In this process, we are retrieving data from a website page using web scraping with the following conditions:
1. The website page can be any retail-themed website ()
2. Data must be extracted using a web scraping method created in a notebook file (.ipynb).
3. The extracted data must include at least 50 rows and 4 columns.

## B. Transform
In the transform stage, we will process the data using Pandas. 
1. Perform a simple data exploration on the data retrieved from web scraping.
2. Check the consistency of data types against the values in each column.
3. Ensure that columns that should contain only numbers, such as price, rating, quantity, etc., have no characters other than numbers and that their data type is numeric.
4. Save the processed data to a .csv file.

## C. Load
At this stage, the processed data is stored in another data storage system, such as a PostgreSQL database.
1. Create a PostgreSQL database based on the processed CSV data. Match the columns and data types with the data.
2. If normalization is required, perform the normalization.
3. Import the CSV data into the PostgreSQL database.
4. The load stage should be executed in a .sql file and run in pgAdmin.
