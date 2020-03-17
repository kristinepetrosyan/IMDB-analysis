# Maximizing our profit in film industry

- [Maximizing our profit in film industry](#maximizing-our-profit-in-film-industry)
  * [Project Info <a name="projectinfo1"></a>](#project-info--a-name--projectinfo1----a-)
    + [Goals](#goals)
    + [The Dataset](#the-dataset)
    + [My Approach](#my-approach)
    + [Technologies](#technologies)
    + [Questions answered and their Recommendations](#questions-answered-and-their-recommendations)
        - [1. How many movies released every year month?](#1-how-many-movies-released-every-year-month)
        - [2. Which month of the year is more profitable?](#2-which-month-of-the-year-is-more-profitable)
        - [3. Which production budget ranges yield the most profitable movies?](#3-which-production-budget-ranges-yield-the-most-profitable-movies)
        - [4. Which genres are the most highly rated and most profitable recently?](#4-which-genres-are-the-most-highly-rated-and-most-profitable-recently)
        - [5. Which directors are making the most profitable movies?](#5-which-directors-are-making-the-most-profitable-movies)

## Project Info <a name="projectinfo1"></a>

    My employer(Microsoft) decided to make a new movie studio without knowing anything about creating movies. They have hired me to help them understand the movie industry and related pros and cons. I am in charge of doing data analysis and presenting what type of movies are doing the best last 10 years.

### Goals
In this project the datasets from IMDb used to explore and understand what type of movies are doing the best in recent years. With provided data we can anser to following questions:
How many movies released each year?
Which month of the year is more profitable?
Which production budget ranges yield the most profitable movies?
What is the runtime duration and genre of top rated movies and which genres are most profitable recently?
Which directors are making the most profitable movies?

### The Dataset
For this project some movie-related data was provided from :
Box Office Mojo
IMDB
Rotten Tomatoes
TheMovieDB.org

### My Approach
Use pandas to initially ingest the datasets
Use pandas to clean columns, convert incorrect column types, add/drop columns, merge different dataframes.
Use seaborn to visualize data.


### Technologies
This project was created using the following languages and libraries.

Python version: 3.6.9
Matplotlib version: 3.0.3
Seaborn version: 0.9.0
Pandas version: 0.25.1
Numpy version: 1.16.5


### Questions answered and their Recommendations


#### 1: How many movies released every year month?


This question will explore which time of the year is preferred for movie releases. 'tmdb_movies_gz' is chosen to search for movie distribution by months and years.
Graph shows figures only in the last ten years since most of the movies are concentrated in this period.

![](./images/Q1-11.png?raw=true)

![](./images/Q1-1.png?raw=true)

We can see that number of released movies increased after 2009 and years 2013, 2014 and 2015 have the highest number of movies.
January and October are the highest in numbers.

##### Recommendation:
2013, 2014 and 2015 has the highest number of movies between 2009 and 2019.
January, October are the top months movies releases happen.

##### Future steps:
More broader dataset can be taken.

#### 2. Which month of the year is more profitable?

'tn_movie_budgets_gz' dataframe is used since it already has release dates and production budget, domestic gross, worldwide gross. Worldwide and Domestic ROI(return on investment) ratio calculated to show each movie's profitability by months. During grouping the ROI ratio by months, the mean () function is used to reach more accurate results.

![](./images/Q2-1.png?raw=true)
![](./images/Q2-2.png?raw=true)


##### Recommendation
June, July and August are the months with highest average both worldwide and domestic ROI,
top 4 months with highest average production budget are May, June, July and November,

##### Future steps:
More concrete insights can be reached with broader datasets including the data of movies released in the past years.

#### 3. Which production budget ranges yield the most profitable movies?
![](./images/PB.png?raw=true)


![](./images/Q3-3.png?raw=true)

##### Recommendation:

I found which budget films lead to profitable films most often. As the plot below show, the more you spend on a given film, the more likely it is to be profitable.
##### Future steps:
More concrete answers can be found by taking more broader dataset which can be scraped.

#### 4. Which genres are the most highly rated and most profitable recently?
![](./images/Q4-1.png?raw=true)

![](./images/Q4-2.png?raw=true)

![](./images/Q4-8.png?raw=true)
![](./images/Q4-4.png?raw=true)

##### Recommendation
We can see that  Action, Adventure, Comedy and Action, Adventure, Sci-Fi are doing the best both domestically and in general. Adventure, Animation, Comedy are the best among highly rated and profitable genres.

We can also see runtime minutes of the movies rated above 7.5. 
We can see that among highly rated movies Adventure, Animation and Comedy are the most profitable.
Most highly rated movies are from 100 to 130 minutes.

##### Future steps:
Further analysis on consumer behavior could be conducted to gain more insights.

#### 5. Which directors are making the most profitable movies?
A director has a lot of impact on making a movie and is required to make decisions which will ultimately affect the profitability of a movie. Let's see which directors are doing the best and whom we should consider hiring.
![](./images/Q5-1.png?raw=true)
![](./images/Q5-2.png?raw=true)

##### Recommendation
Top 2 directors with the most profit are Travis Cluff and Chris Lofing who did well both worldwide and domestically.

##### Future steps:
Further analysis on consumer behavior could be conducted to gain more insights.




