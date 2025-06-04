# Implementation-of-Movie-Recommender-System---Python
Recommender systems are tools designed to suggest items that align closely with a user's interests by analyzing their historical interactions and preferences. These systems are widely applied in domains such as movie and music recommendations, personalized news feeds, and search engines. There are two primary techniques for generating these recommendations:

Collaborative Filtering: This method relies on the behavior and preferences of users to suggest items. It identifies users with similar tastes and recommends items that those users have liked. For instance, if User A enjoys movies X and Y, and User B likes movies Y and Z, the system may infer that User A could also be interested in movie Z.

Content-Based Filtering: This approach focuses on the characteristics of items and the individual user’s prior preferences. If a user tends to watch action movies, the system will suggest other action films by analyzing aspects such as genre, cast, or director.

In this article, we’ll demonstrate how to build a simple movie recommendation system in Python that uses a user’s viewing history to suggest new films they might enjoy.
Step 1: Import Libraries and Load the Data
In this step we will load pandas ,matplotlib and seaborn library. After that we will load user ratings for movies file. Each row in this file shows a user’s rating for a specific movie. To download file click here: .tsv file.
Step 2: Loading Movie Titles
Now we load another file that matches movie IDs to their titles. This helps us show the actual movie names instead of just numbers. You can download file from here: Movie_Id_Titles.csv.
Step 3: Merging Both Datasets
We now combine the data about user ratings and movie titles and we can see both the movie names and the ratings for each movie.
Step 4: Analyzing Movie Ratings
This gives us the average rating for each movie and use to find top-rated movies.
Step 5: Creating a Ratings DataFrame
In this step the DataFrame stores the average rating and number of ratings for each movie. We’ll use this later to filter out movies with few ratings.
Step 6: Visualizing Ratings
We use matplotlib and seaborn to create visual charts that make the data easier to understand
 Step 7: Creating User-Movie Matrix
We now create a matrix where each row represents a user and each column represents a movie. The values in this matrix are the ratings that users have given to each movie.
Step 8: Finding Similar Movies
We compare how users rated other movies vs. "Star Wars (1977)". corrwith() calculates correlation with all other movies.
Step 9: Filter Movies with Enough Ratings
Join the correlation data with our ratings dataframe. Filter movies that have more than 100 ratings for more reliable recommendations.
Step 10: Trying Another Example
Same process as before now checking for movies similar to “Liar Liar (1997)”.
