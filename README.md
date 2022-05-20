# Movies-ETL

# Project Overview

This project will look at updating Amazing Prime daily by creating an automated pipeline that will take in new data, perform transformations, and load the data into existing tables. 
One function would be created and refactored to take in three files Wikipedia data, Kaggle metadata, and the MovieLens rating data.
Lastly an ETL is performed by adding the data to a PostgreSQL database.

# Resources

Python, Pandas, PostgreSQL, Jupyter Notebook
Data Source: wikipedia-movies.json, movies_metadata.csv, ratings.csv

# Results

The following steps would be followed for this analysis:

•	Deliverable 1: Write an ETL Function to Read Three Data Files

Write a function that reads in the three data files and creates three separate DataFrames.
 

 ![image](https://user-images.githubusercontent.com/96086671/169589598-f4f83d8c-0713-4bcb-8a14-c4ef7be986a4.png)


 ![image](https://user-images.githubusercontent.com/96086671/169589631-d8350397-08e1-4c55-ab59-d079fa6a0ffe.png)


![image](https://user-images.githubusercontent.com/96086671/169589689-2f095e84-d62c-4336-b3ee-98e75dd57e5a.png)


•	Deliverable 2: Extract and Transform the Wikipedia Data

Extract and transform the Wikipedia data so it can be merged with the Kaggle metadata. Also extract the IMDb IDs using a regular expression string and dropping
duplicates, use a try-except block to catch errors.
 

 ![image](https://user-images.githubusercontent.com/96086671/169589760-7d09e061-09ac-49d0-a774-e94fa592d117.png)


![image](https://user-images.githubusercontent.com/96086671/169589829-8539ae40-b9bd-4ca5-a596-5c85c9a77d43.png)


•	Deliverable 3: Extract and Transform the Kaggle data

Extract and transform the Kaggle metadata and MovieLens rating data, then convert the transformed data into separate DataFrames. Also merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.
 

 ![image](https://user-images.githubusercontent.com/96086671/169589921-4e75ffab-8592-4138-a966-48eb03ee6214.png)


 ![image](https://user-images.githubusercontent.com/96086671/169589990-2d2b7a42-cb9c-443c-ac26-fa652745137f.png)


![image](https://user-images.githubusercontent.com/96086671/169590042-9ab858f3-2723-4e76-9af8-230ef8a94d8f.png)


•	Deliverable 4: Create the Movie Database

Add the movies_df DataFrame and MovieLens rating CSV data to a SQL database.
 
 
 ![image](https://user-images.githubusercontent.com/96086671/169590116-acc28e5b-30db-49ce-a1c5-a398a0db0065.png)


![image](https://user-images.githubusercontent.com/96086671/169590158-d0234bb2-73e4-441c-88ac-bae42a6a1255.png)


# Summary

The ETL function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
