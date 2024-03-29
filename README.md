# Movies-ETL

## Overview of ETL process
 * This project is aiming to create a function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data, then performs the ETL process to load the data into a PostgreSQL database. 
1.  Write a function extract_transform_load(ETL) that reads in the three data files from appropriate paths. 
2.  Convert three files to separate Pandas DataFrames.
3.  Clean up Wikipedia data and Kaggle metadata. Including dropping and combining columns, removing missing data, changing data type, and formatting messing data with Regex.
4.  Merge cleaned wiki_movies_df and kaggle_metadata to a new data frame movies__df.
5.  Transform and merge the ratings DataFrame into movies__df to get movies_with_ratings_df.
6.  Add movies_df DataFrame and MovieLens rating CSV data to a SQL database. Check movies table and ratings tabel to comfirm the import.

## Results
  - **Data frames**
    1. wiki_movies_df data frame![wiki_movies_df](https://user-images.githubusercontent.com/105877888/182679583-070c02e3-9995-46d8-9904-6a714e47c8dd.PNG)
    2. movies_df data frame ![movies_df](https://user-images.githubusercontent.com/105877888/182679601-b4a508f5-4bb2-4127-b2de-85932001483a.PNG)
    3. movies_with_ratings_df dataframe ![movies_with_ratings_df](https://user-images.githubusercontent.com/105877888/182679619-4b17259f-739e-405e-bea8-312b2cc15ff1.PNG)

- **Import into SQL Movie database**
    1. ETL processing
  ![ratings_importing](https://user-images.githubusercontent.com/105877888/182679870-1517bfed-c79a-48e6-8d35-c36a1915f103.PNG)

    2. Movies table
![movies_query](https://user-images.githubusercontent.com/105877888/182679911-491f9faa-ca24-4431-9655-736b67fe1a74.PNG)

    3. Ratings tabel
![ratings_query](https://user-images.githubusercontent.com/105877888/182679921-8e63a4ff-50de-4305-a003-99e53bb1ef5f.PNG)


## Summary
  - Three file resouces with two different file types(csv and json files) were all imported into pandas library. File data were cleaned up with various method and converted into data frames, which were easier to read. 
  - All useful data were imported into SQL database. This is a convenient way to hold the meta data.
  - To do more specific researches about on movie data, we can do neccessery queries from Movie database and export the results later. 
