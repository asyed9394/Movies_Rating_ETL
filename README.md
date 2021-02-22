# IMDB movies and rating ETL

## Project Overview
"Amazing prime" is a company that provides online video and movie streaming . The company decided to run a hacathon open to data science community . 
The purpose of hackathon to predict a movie populairy for low budgest films, so "Amazing Prime" can buy the rights for these movies and improve its ROI

In order to support data scientist , the data team is going to create a movie database and publish it in a psotgress for the analysis. 

### Data sources

- Wikipedia data for movies from 1990 to 2018:
	Wikipedia has a ton of information about movies, including budgets and box office returns, cast and crew, production and distribution, and so much more.
	
- Use Rating data available online rather than from the company's app. 	So the dataset found on Kaggle that contains ratings data from MovieLens, a site run by the GroupLens research team.
	This data is available as part of Kaggle's [The IMDB Movie database TMDB](https://www.themoviedb.org/)


### Challenge:
- Extract and load data into python data forames to data , build tranformation and data cleaning logic. Enrich data about movies by combining Kaggle and Wikipedia movies data.
- Transform : Write python functions to clean, merge and trasnform data into usable format
- Load int the database : load data into the database
Write code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.


#### Assumption:

 Assume new files replace the contents of previously processed files compeltly.


## Resources
- Data source: 
     - [Wikipedia Movie Data JSON file format](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_8/wikipedia-movies.json)
     - [Movide database zip file](https://www.kaggle.com/rounakbanik/the-movies-dataset/download)
		Out of 7 files found in the database , we are interested in two files only.
		1.movies_metadata.csv
		2.ratings.csv
    
- Software: Anaconda Jupyter notebook Python 3.7 , panda ,sqlalchemy, psycopg2
- Database : Postgress 11.6
- Final ETL code: [ETL Code to transform and load movie data](ETL_create_database.ipynb)
- Row counts in final movie database

Note: The data files are not loaded to Git due to the size. Data files can be donwloaded from the links provided above.

### Row count in movie table:

![Row counts in movies table](/Resources/movies_query.png)
	

### Row count in Ratings table:

![Row count in rating table](/Resources/ratings_query.png)
	
	


