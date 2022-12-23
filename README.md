# Data Analysis of a Movie Database

The movie database (TMDB) is a database that contains informations of about 10,000 movies which was gotten from kaggle. The database is made up 21 features. These are,  id, imdb_id, popularity, budget, revenue, original_title, cast, homepage, director, tagline, overview, runtime, genres, production_companies, release_date, vote_count, vote_average, release_year	, budget_adj, and revenue_adj. From the proper inspection of the data, the following questions were coined out based on the features.  

Questions:
* Popularity  
* Director  
* Profit  
* Release year  

## Conclusions  

> The dataset lacked consistency. The data wrangling process consisted of dropping the null values, renaming and reordering the features (columns). The null values in the dataset was dropped because they were so little compared to the overall sample data. The zero values in the features were filled with null values so as to protect the data intergrity as they were so ambigious and dropping them would result in losing more than half of the sample data collected. The features were also renamed and reordered for clarity. 

> The profit feature generated was computed by subtracting the budget from revenue. This was to ensure proper evaluation of coined research questions. The profit feature at the 75% percentile was set to be the margin for high profitability while that of 25% percentile was the margin for low profitability. The rating feature was found to be the dependent variable as it has a relatively normal distribution when compared to the other features.

> For the ease of analysis, research questions were coined out based on the features of the dataset. In the first case, the popularity feature was addressed. From the distribution, about 90% of the movies released were not popular. In analyzing how profitable the top 200 most popular movies are; about 49% of the movies were profitable. Indicating that there is no so much correlation in profit compared to their popularity. Also, in terms of rating the popularity showed no relationship in the scattered plot.

> In the case of the director feature, Colin Trevorrow was the most popular director and he directed only two movies which made him popular in return. Also, Woody Allen was the director with the highest number of movies released. He released 46 movies with only one being highly profitable.

> In the case of the profit feature, most movies made profit within 0 - 100 Million. However, the movie with the highest profit generated was Avatar. In terms of rating, profitability showed no correlation.

> Finally, in the case of the release_year feature, most of the movies were released within 2010 - 2015. However, 2014 was the year with th highest number of movies released. A total of 680 movies were released.  

## Limitations  

> The movie database (TMDB) contains one of the best collection of movies. Most feautures (columns) had null values and lots of outliers. The outliers in most features were out of range, making comparism between features very difficult. Furthermore the features had thousands of zero values. For example the budget and revenue features had 5,578 and 5,888 respectively. However, the zero values was not dropped but replaced with null values to protect the data intergrity. This lack of consistency in the dataset caused some set backs in the analysis carried out.  

## Reference  

The following are the links to the resources utilized in carrying out the analysis of the movie database (TMBD):

> + [The most influential factor of IMDB movie rating](https://medium.com/@yd334/the-most-influential-factor-of-imdb-movie-rating-part-ii-data-analysis-and-statistical-modeling-c6300b8d7d4d)  
> + [What makes a movie hit a jackpot](https://towardsdatascience.com/what-makes-a-movie-hit-a-jackpot-learning-from-data-with-multiple-linear-regression-339f6c1a7022) 
> + [The TMDB 5000 movie dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)  
> + [TMDB movies analysis](https://www.kaggle.com/code/betizazualemu/tmdb-movies-analysis-ipynb)  
> + [Pandas DataFrame groupby function for grouping features](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.groupby.html)  
> + [How to plot a pandas dataframe with matplotlib](https://www.geeksforgeeks.org/how-to-plot-a-pandas-dataframe-with-matplotlib/)  
> + [The query function in pandas dataframe](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.query.html)  
> + [Dropping null values in pandas dataframe](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.dropna.html)  
> + [Exploding elements in pandas dataframe](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.explode.html)

