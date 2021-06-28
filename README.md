# Amazing Prime Video-Movie ETL-Analysis

## Overview of Project

Amazing Prime Video is a part of Amazing Prime. It is a streaming service which streams movies and television shows for the viewers.
They want to develop an algorithm to find out which low budget movies would be popular, so that they can buy the streaming rights for those movies for a bargain.
For this purpose they have decided to sponsor a hackathon, where they plan to provide a clean set of data for the participants to predict the most popular movies.
The purpose of this project is to help generate these clean sets of data.

## Purpose


The preliminary data is present in one json and two comma separated values(CSV) files.
The json file is: wikipedia-movies.json which has the Wikipedia movies data
The CSV files are: ratings.csv which has the ratings data and movies_metadata.csv which have the Kaggle movies data.

The purpose of this project is to provide the below deliverables:

Deliverable 1: Write an ETL Function to Read Three Data Files
Deliverable 2: Extract and Transform the Wikipedia Data
Deliverable 3: Extract and Transform the Kaggle data
Deliverable 4: Create the Movie Database

## Results

Deliverable 1: Write an ETL Function to Read Three Data Files
The function to read the three files has been written:
![Screen Shot 2021-06-28 at 12.38.17 PM](https://i.imgur.com/xFf6Hdj.png)

Deliverable 2: Extract and Transform the Wikipedia Data
The Wikipedia data has been extracted and transformed.

The Wikipedia data has been transformed to filter out the TV shows.
The required IMDB IDs have been taken from the data.
The dollar amount, budget, release date and running time data have been filtered, formatted and transformed to hold data in the same format.

A sample of the data is as below:
![Screen Shot 2021-06-28 at 12.59.25 PM](https://i.imgur.com/0Urs9ce.png)
![Screen Shot 2021-06-28 at 12.59.56 PM](https://i.imgur.com/JGfvp5J.png)

Deliverable 3: Extract and Transform the Kaggle data
The Kaggle Data has been extracted and transformed.

The adult movie titles have been dropped.
The video, budget, id, popularity data have been filtered, formatted and transformed to hold data in the same format.
The Wikipedia and Kaggle Data frames have been merged into one.

![Screen Shot 2021-06-28 at 12.58.28 PM](https://i.imgur.com/zZ39dgK.png)

![Screen Shot 2021-06-28 at 12.59.00 PM](https://i.imgur.com/7akBmLL.png)

Deliverable 4: Create the Movie Database

The movie database has been created.
The movies and ratings tables have been created.

The movies table data:

![Screen Shot 2021-06-28 at 1.01.03 PM](https://i.imgur.com/WmSfNlH.png)

The ratings data is as below:

![Screen Shot 2021-06-28 at 1.10.00 PM](https://i.imgur.com/fMuWZAf.png)

The DB details are as below:

![Screen Shot 2021-06-28 at 1.10.35 PM](https://i.imgur.com/6dr5T5h.png) 

# Amazing Prime Video-Movie ETL-Summary

The Wikipedia, Kaggle and Ratings data have been cleansed, transformed and loaded into Postgres tables. This has been done using ETL functions and by creating a pipeline which extracts, transforms and loads data. The data in the Postgres tables can be used in the hackathon