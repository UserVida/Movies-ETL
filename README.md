<<<<<<< HEAD
# Overview of Project - Movies ETL

## Purpose
The purpose of this project was to create a singular clean dataset of movie data to be used in a company presented hackathon. 

## Technologies Used:
Python- Pandas
PostgreSQL

## Procedure
The data used in this project was extracted from 3 sources:

•	Movie data scraped from Wikipedia
•	Movie dataset from Kaggle
•	Rating data scraped from MovieLens

The data was then transformed to remove unnecessary columns and rows and to organize the data values and columns. Once all the data from each data source was cleaned, the dataframes were merged into one dataset using a left join. Duplicate columns were dropped and missing values in one column were filled in using the duplicate column in from the second dataframe. The final dataframe was then loaded into a SQL database, ready for use.

## Results 

![Screenshot 2022-11-13 at 22-18-05 ETL_function_test - Jupyter Notebook](https://user-images.githubusercontent.com/97644424/201568099-b6c0c381-1f55-43bf-a62e-4911df7b41f0.png)

A function was written to read in three separate data files and convert these files into three dataframes. 

![Screenshot 2022-11-13 at 22-51-08 ETL_clean_wiki_movies - Jupyter Notebook](https://user-images.githubusercontent.com/97644424/201816051-233501f4-9c55-4906-8073-2a702015c026.png)

The code was further refactored to remove unnecessary columns from the Wikipedia data file. The cleaned file was then turned into a dataframe. Then regular expression strings were used to drop duplicates in the imdb_id column and a try and except block was used to catch any errors.

More code was added after to clean the box_office, budget and release date column from the wiki_movies_df dataframe.

![Screenshot 2022-11-14 at 22-23-53 ETL_clean_kaggle_data - Jupyter Notebook](https://user-images.githubusercontent.com/97644424/201819119-50059255-5003-4291-b980-cda4fed89f0a.png)

The Kaggle metadata and MovieLens rating data files were extracted and transformed to create separate dataframes. The Kaggle metadata dataframe was merged with the Wiki movies dataframe to create the new dataframe movies_df. Then columns from the MovieLens rating dataframe were merged with movies_df to create the final dataframe, movies_with_ratings_df. 

<img width="676" alt="movies_query" src="https://user-images.githubusercontent.com/97644424/202077167-f7e5d096-1657-46c7-9a8a-5b8c45690e5d.PNG"> <img width="678" alt="ratings_query" src="https://user-images.githubusercontent.com/97644424/202077182-093f44f8-c630-4ea3-b0aa-936f9e6459f1.PNG">

In this final section of code, the movies_df dataframe and MovieLens rating csv data was added to a SQL database. A query was then run on the Postgre SQL database to retrieve the number of rows for the movies and ratings table to ensure that all the data was successfully added. 

### Authors
•	Zainab Cheentavida
=======
# Overview of Project 

## Purpose 

The purpose of this project was to create a singular clean dataset of movie data to be used in a company presented hackathon. The data used in this project was extracted from 3 sources:

* Movie data scraped from Wikipedia
* Movie dataset from Kaggle
* Rating data scraped from MovieLand 

The data was then transformed to remove unnecessary columns and rows and to organize the data values and columns. Once all the data from each datasource was cleaned, the dataframes were merged into one dataset using a left join. Duplicate columns were dropped and missing values in one column were filled in using the duplicate column in from the second dataframe. The final dataframe was then loaded into a SQL database, ready for use.
>>>>>>> f6979318c5a345ff5acf9219eb6b08a55152f2f8
