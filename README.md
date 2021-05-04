# Movie Data Analysis Project

## Overview
Microsoft wants to enter into the world of film industry by opening a movie studio for which Microsoft need to make a key decision in order to succeed in the film industry. This is accomplished by exploring what type of films are currently doing the best at the box office, and then translating those findings into actionable insights for Microsoft.



## Business Problems
Microsoft is stepping into film industry by creating a new movie studio but as this is the beginning of their journey they might not have an proper understanding and without knowing the current market and audience could lead to failure which would be both embarrassing for the company and result in a loss of money. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.

## Data
The  **datasets**  folder contains the datasets used for this project:

 - tn.movie_budgets.csv
 - imdb.title.basics.csv
 - title.ratings.csv
 - imdb.title.principals.csv
 - final_df.csv

`tn.movie_budgets.csv`  is used to get the movie budget and worldwide gross.
`imdb.title.basics.csv` is used to get the title of the movies.
`title.ratings.csv` is used to get movie ratings.
`imdb.title.principals.csv` is used to get director associated with the movie.
`final_df.csv` is the final dataset generated after data cleaning process which is further used to produce actionable insights.

## Questions
### Q1.  Which are the Most Profitable Genres ?
#### Observation 1:
In order to see which genre has most movies we group by genre and counted the total movies made with the data which was available.
![TOTAL MOVIES BY GENRES](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/total_movies_genre.jpg?raw=true)
#### Observation 2:
 Minimum, Maximum and Average Return on investment (ROI) by each Genre.
 ![enter image description here](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/mean_max_min_roi_genre.jpg?raw=true)
#### Observation 3:
Variation of Average Ratings by each Genre
![enter image description here](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/rating_genre.jpg?raw=true)

### Q2.  What is the ideal Budget, Based on Genre ?
From the Above finding we found based on Ratings and ROI we limiting our exploration to only the top 3 genres.
To find out the ideal budget which by Genre which has good ROI we categorized budgets into 5 class.
Ultra Low (1M - 10M)
Low (10M - 25M)
Mid (25M - 50M)
High (50M - 100M)
Ultra High (100M+)
![enter image description here](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/roi_budget_class.jpg?raw=true)
### Q3.  ## Who are the most profitable Directors ?
In order to find top director who have given Hit movies that had a very good ROI we filtered out the top directors based on average ROI.
