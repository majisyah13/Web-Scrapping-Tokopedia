# Web-Scrapping-Tokopedia

# Project Overview
This project demonstrates how to perform web scraping on an e-commerce website in Indonesia, specifically Tokopedia. The example provided is scraping data on "seblak" products listed on Tokopedia.

## A. Extract
The first stage in the data pipeline is `Extract`. In this process, we are retrieving data from a website page using web scraping with the following conditions:
1. Using Selenium WebDriver and BeautifulSoup to retrieve data from Tokopedia pages
2. Retrieving data on "seblak" products listed on Tokopedia
 
## B. Transform
In the transform stage, we will process the data using Pandas. 
1. Perform a simple data exploration on the data retrieved from web scraping.
2. Check the consistency of data types against the values in each column.
3. Ensure that columns that should contain only numbers, such as price, rating, quantity, etc., have no characters other than numbers and that their data type is numeric.

## C. Load
At this stage, the processed data is stored in another data storage system, such as a PostgreSQL database.
1. Transform dataframe into tuple.
2. Dump scrapped data to postgreSQL
