# NYC Airbnb Data Cleaning & Analysis

## Project Overview

This project focuses on cleaning and analyzing the **New York City Airbnb Open Data** dataset using **Python, Pandas, and NumPy**.

The main goal was to improve data quality, handle missing and invalid values, identify price outliers, and perform exploratory data analysis to discover useful patterns in Airbnb listings.

## Tools & Technologies

* Python
* Pandas
* NumPy
* Google Colab / Jupyter Notebook

## Dataset

The dataset contains information about Airbnb listings in New York City, including:

* Listing details
* Host information
* Neighbourhood and borough
* Room type
* Price
* Minimum nights
* Number of reviews
* Last review date
* Reviews per month
* Availability

## Data Cleaning

The following cleaning steps were performed:

* Checked the dataset structure and data types
* Checked for missing values
* Checked for duplicate records
* Removed 11 listings with a price of $0
* Converted `last_review` to datetime format
* Replaced missing `name` and `host_name` values with `Unknown`
* Replaced missing `reviews_per_month` values with 0
* Created a `has_review` column to identify listings with and without reviews
* Used the IQR method to identify unusually high prices
* Created a `price_status` column to flag price outliers
* Performed final data validation

## Exploratory Data Analysis

The analysis examined:

* Room type distribution
* Listings by neighbourhood group
* Average price by room type
* Average price by neighbourhood group
* Average price by room type and neighbourhood group
* Top 10 most expensive listings
* Top 10 neighbourhoods by listing count
* Average minimum nights by room type
* Average availability by room type
* Average reviews by room type
* Top 10 neighbourhoods by average price
* Relationship between price and number of reviews
* Top hosts by number of listings
* Review status distribution

## Key Findings

* The cleaned dataset contains **48,884 listings**.
* **Entire home/apt** has the highest average price at approximately **$211.81**.
* **Manhattan** has the highest average listing price at approximately **$196.88**.
* **Williamsburg** has the highest number of listings with **3,919 listings**.
* Manhattan has the largest number of listings with **21,660 listings**.
* Shared rooms have the highest average availability at approximately **161.87 days**.
* Private rooms have the highest average number of reviews at approximately **24.10 reviews**.
* **Sonder (NYC)** has the highest number of listings among the analyzed hosts, with **327 listings**.
* Approximately **79.4%** of listings have review history, while **20.6%** have no review history.
* The correlation between price and number of reviews is very weak and negative (**-0.0479**).

## Project Files

* `NYC_Airbnb_Data_Cleaning_Analysis.ipynb` — Complete Python data cleaning and analysis notebook
* `cleaned_airbnb.csv` — Final cleaned dataset
* `README.md` — Project documentation

## Conclusion

This project demonstrates practical data cleaning and exploratory data analysis using **Python, Pandas, and NumPy**. The dataset was inspected, cleaned, validated, and analyzed to identify patterns related to Airbnb pricing, room types, locations, reviews, availability, and hosts.
