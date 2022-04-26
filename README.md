# movie-data-visualization
Dataset used
I have used the MovieLens Dataset. That data I have used consists of 105339 ratings in the ratings.csv file, applied over 10329 movies in the movies.csv.

Essential Libraries
recommenderlab, ggplot2, data.table and reshape2.

Data Pre-processing
After retrieving data from the movies.csv andratings.csv datasets, I observed that the userId column, as well as the movieId column, consisted of integers. Furthermore, I needed to convert the genres present in the movie_data dataframe into a more usable format by the users. In order to do so, I first created a one-hot encoding to create a matrix that comprises of corresponding genres for each of the films. I then created a search matrix that will allow us to perform an easy search of the films by specifying the genre present in our list.

There are movies that have several genres. For the movie recommendation system to make sense of the ratings through recommenderlab, I convert the matrix into a sparse matrix. This new matrix is of the class realRatingMatrix. I then overviewed some important parameters that provided various options for building recommendation systems for movies.

Collaborative Filtering - Exploring similar data
Collaborative Filtering involves suggesting movies to the users that are based on collecting preferences from many other users. For example, if a user A likes to watch action films and so does user B, then the movies that the user B will watch in the future will be recommended to A and vice-versa. Therefore, recommending movies is dependent on creating a relationship of similarity between the two users. With the help of recommenderlab, I computed similarities using various operators like cosine, pearson as well as jaccard.

Visualisation: Similarity in data
I visualised the similarity between the users as explained in the above section as well as the similarity shared between the films.

Visualisation: Most viewed movies
In this section of the machine learning project, I explored the most viewed movies in the dataset. Before this, I counted the number of views in a film and organized them in a table that would group them in descending order. I visualized the total number of views of the top films as a bar plot.

From the visualisation, it could be observed that 'Pulp Fiction' is the most watched film followed by 'Forrest Gump'.

Visualisation: Heatmap of Movie Ratings
Now, in this data science project of Recommendation system, I visualized a heatmap of the movie ratings. This heatmap will contain first 25 rows and 25 columns.

