# Movies-ETL

## Purpose:
The purpose of this project is to create an Extract Transform & Load (ETL) pipeline of movie data from muultiple raw data sources to an SQL database using Python, Pandas, Regex, and Postgres SQL. 

## The Process:
Two data sets were collected, the first is a scraped wikipedia data set containing JSON formatted information about movies from 1990-2018. The second dataset is Kaggle based dataset including ratings from MovieLens. 

Cleaning the Wikipedia dataset included writing a two functions in python. The first is a Clean_Movie function to clean up multiple language titles and column names. The second function, called Extract_Transform_Load, imports both datasets and applies a series of transformations to create consistent, usable data. Some of the Transformation processes are to filter TV shows, remove duplicates, and use Regular Expressions to clean up box office and budget monetary, and run times in the wikipedia dataset. The ETL function also cleaned the kaggle dataset to remove adult movies, modify column types and change release dates to datetime. Three dataframes were returned, including: wiki_movies_df, movies_df, and movies_with_ratings_df. The datasets were then merged and imported into a postgres SQL database to be queried. 

Focus of the project was aimed at honing ETL skills using python functions and pandas to manipulate data. 
