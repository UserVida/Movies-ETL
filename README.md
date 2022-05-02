# Overview of Project 

## Purpose 

The purpose of this project was to create a singular clean dataset of movie data to be used in a company presented hackathon. The data used in this project was extracted from 3 sources:

* Movie data scraped from Wikipedia
* Movie dataset from Kaggle
* Rating data scraped from MovieLand 

The data was then transformed to remove unnecessary columns and rows and to organize the data values and columns. Once all the data from each datasource was cleaned, the dataframes were merged into one dataset using a left join. Duplicate columns were dropped and missing values in one column were filled in using the duplicate column in from the second dataframe. The final dataframe was then loaded into a SQL database, ready for use.
