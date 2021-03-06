# Movie Data Analysis Project
![Movie Theater](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/theater.jpg?raw=true)
## Overview
Microsoft wants to enter into the world of film industry and needs an effective business strategy based on which films are doing well and are successful at box office.

## Business Problems
 - Making a film without doing market analysis could result in loss and business failure.
 - Ideal budget to be considered in order to at least break even.
 - Director to be considered based on Genre of the film.


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
 ![ROI RANGE BY GENRES](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/mean_max_min_roi_genre.jpg?raw=true)
#### Observation 3:
Variation of Average Ratings by each Genre
![RANGE OF RATINGS BY GENRES](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/rating_genre.jpg?raw=true)

### Q2.  What is the ideal Budget, Based on Genre ?
From the Above finding we found based on Ratings and ROI we limiting our exploration to only the top 3 genres.
To find out the ideal budget which by Genre which has good ROI we categorized budgets into 5 class.
Ultra Low (1M - 10M)
Low (10M - 25M)
Mid (25M - 50M)
High (50M - 100M)
Ultra High (100M+)
![ROI BY BUDGET CLASS](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/roi_budget_class.jpg?raw=true)
### Q3.  ## Who are the most profitable Directors ?
In order to find top director who have given Hit movies that had a very good ROI we filtered out the top directors based on average ROI.
![AVERAGE ROI BY DIRECTOR](https://github.com/avithekkc/P1-moive-data-analysis/blob/main/images/avg_roi_director.jpg?raw=true)
##  Conclusions
Based on the data available I would recommend Microsoft to to make a movie that has ultra low or low budget on a Thriller Drama Movie with one of the following Directors

 - John R. Leonetti
 - James Wan
 - Scott Derrickson
 - Christopher Landon
 - David F. Sandberg

## Next Steps

 - We had limited data to do the analysis and to meet our criteria we drop few rows to boost the result. we could use API's to gather large amount of data and do the same analysis to get better results.
 - Analysis on successful Producers, Cinematographers, Writers and Actors.
 - Removing movies that had a clash with big budget movies which resulted into failure as this might give false indications on our predictions and recommendation.
 - Analysis on Soundtrack as can also help making a movie hit.
 - Filter out movies by language.


##   Repository Structure
```
????????? datasets                            <- All the data used for the analysis.
????????? images                              <- All images used throughout the project.
????????? data-cleaning.ipynb                 <- Cleaning of data to create final dataset (part 1).
????????? data-visualization.ipynb            <- Insights and analysis (part 2).
????????? presentation.pdf                    <- PDF version of project presentation.
????????? readme.md                           <- README file for Quick overview on project.
```
