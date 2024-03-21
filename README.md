# MOVIE DATA ANALYSIS FOR MICROSOFT MOVIE STUDIO



## Project Overview

For this project, we will use exploratory data analysis to generate viable and actionable insights for Microsoft as they want to venture into movie production.

### Business Problem

Microsoft, a big Tech. company has seen all the big companies creating original video content, and wants to expand its scope into creation of video content like the other companies.They have decided to create a new movie studio, but they know so little about movie creation. <br/>
We are now tasked with the responsibility to explore the box office and check which films are currently at the top. Afterwards we are required to recommend viable insights to Microsoft, for its new movie studio based on the findings we have gotten, to help them in their movie production. <br/>
We try to generate responses for the following hypothesis:
### Hypothesis
 1. Which genres of movies having a high rating should Microsoft venture into their production?

 2. How much should Microsoft budget in the production of the movies? The correlation between the production budget 
    and the domestic and worldwide gross amounts

 3. Which month should the movies be released in order to be popularity?


## Data Understanding

The Data we are going to use in our data exploration is contained in two csv files and a database file contained in the `zippedData folder`. The database file also has several tables but we are only interested in two tables.
 1. `tn.movie_budgets.csv` : Contains information about the movies produced with their production budget, domestic gross and worldwide gross estimates collected from [The Numbers](https://www.the-numbers.com/).
 2. `tmdb.movies.csv` : This dataset contains general information about the movies produced such as original_title, release date, popularity, etc which was collected from [TheMovieDB](https://www.themoviedb.org/).
 3. `im.db` : This is an SQLite database containing the tables `movie_basics` and `movie_ratings` which are of most importance collected from [IMDB](https://www.imdb.com/).
 
This data may not be upto date as of this time currently. You will need to look carefully at the features to figure out how the IMDB data relates to the other provided data files.

## Data Analysis 

For our three hypothesis that we are trying to answer, in order to get accurate analysi results, we need to clean the data and ensure there are no missing data and ensure the data is in the correct format and datatypes for easier use. 


## Project Findings
After our analysis of the data, we got this findings:
 1. There are some movie genres that Microsoft should consider to produce as they venture into film production since they have recieved higher ratings from the public. Comedy, Documentary, History is the highest rated genre.
 ![Genre vs Rating Relationship](https://github.com/EdmundNyaribo/dsc-phase-1-project-movie-data-analysis/blob/master/images/hypothesis1Finding.png)
 
 2. There is a moderate to strong positive relationship about the cost of production and the gross returns the movie would generate. Hence a higher realistic budget will yield higher gross returns both in the domestic and worldwide market.
* Production budget and Domestic gross have a correlation coefficient of 0.6857.
 ![production budget vs domestic gross](https://github.com/EdmundNyaribo/dsc-phase-1-project-movie-data-analysis/blob/master/images/hypothesis2.1Finding.png)
* Production budget and worldwide gross have a correlation coefficient of 0.7483.
 ![production budget vs worldwide gross](https://github.com/EdmundNyaribo/dsc-phase-1-project-movie-data-analysis/blob/master/images/hypothesis2.2Finding.png)
 
  3. From our analysis we can found that movies released in the months of December, July and August have a higher popularity. Movies released in January are not that popular.
 ![Release month popularityS](https://github.com/EdmundNyaribo/dsc-phase-1-project-movie-data-analysis/blob/master/images/hypothesis3Finding.png)


## Conclusion
### Recommendations

From the analysis we have done on the provided datasets, we can provide the following recommendations to Microsoft to guide them in their movie production quest: 
 1. Microsoft should release movies of the top genres which have the highest rating by the public. These genres have proved to be liked by the public than the other genres. I would recommend producing movie genres that have a rating of 6.9 and above.
* Comedy, Documentary, Fantasy
*  Documentary, Family, Musical
*  History, Sport
*  Game-Show 
*  Music, Mystery etc. 
 
 2. In terms of the production budget, I would recommend Microsoft to invest a good amount of finances in the production of the movies. This is because there is a positive correlation between the production budget and the domestic gross as well as the worldwide gross.
 
 3.  Microsoft should consider releasing a movie in the months of December, July or August. These Months have shown to yield the highest popularity of a movie.
