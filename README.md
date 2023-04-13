# pyspark-analysis
 
Objectives:
The objective of the project was to explore the available sample data from IMDB using Apache Spark and Spark's Dataframes API. Exploratory data analysis was performed to answer questions about movies, such as the most frequent genre of titles, the number of different movie titles, the average duration of adult content movies, the number of movies with current title different from the original title, the longest movie title, the movie with the highest number of votes, and the lowest average rating of a movie.

Analysis:
To perform the data analysis, the "title_basics.tsv" and "title_ratings.tsv" files were read using Spark's Dataframes API. Then, the following analyses were conducted:

What is the most frequent genre of titles?
To answer this question, a new dataframe was created by grouping the data by genre and counting the number of titles in each genre. Then, the data was sorted in descending order to find the most frequent genre.

How many different movie titles exist?
A new dataframe was created containing only the unique movie titles, and then the number of titles in the dataframe was counted.

What is the average duration of adult content movies?
A new dataframe was created containing only the movies with an "adult" age rating, and then the average duration of these movies was calculated.

How many movies have the current title different from the original title?
A new dataframe was created containing only the movies whose current title is different from the original title, and then the number of movies in the dataframe was counted.

Which movie has the longest title?
A new dataframe was created by sorting the data by title length in descending order, and then the first record in the dataframe was selected to obtain the longest movie title.

Which movie has the highest number of votes?
A new dataframe was created by sorting the data by the number of votes in descending order, and then the first record in the dataframe was selected to obtain the movie with the highest number of votes.

What is the lowest average rating of a movie?
A new dataframe was created containing only the movies with an assigned average rating, and then the minimum average rating of these movies was calculated.

Conclusion:
The project used Spark's Dataframes API to explore the available sample data from IMDB. Data analysis allowed for answering questions about movies and extracting relevant information from the dataset. The use of Spark allowed for quick and scalable analysis, even for large-sized files.