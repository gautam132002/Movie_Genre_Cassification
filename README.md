# Movie Genre Prediction using Logistic Regression

This repository contains a Python script for collecting movie data from The Movie Database (TMDb) API and using logistic regression to predict movie genres based on the collected data.

## Data Collection

### TMDb API Endpoint
We collect movie data from the TMDb API using the following endpoint:
```
https://api.themoviedb.org/3/discover/movie?include_adult=true&include_video=false&language=en&page={page_no}&language=en
```

### Data Fields
We accept the following data fields for each movie from the API response:
- `adult`: Whether the movie is rated as adult (True or False)
- `backdrop_path`: URL of the movie's backdrop image
- `genre_ids`: Comma-separated list of genre IDs associated with the movie
- `id`: Unique identifier for the movie
- `original_language`: Original language of the movie
- `original_title`: Original title of the movie
- `overview`: Overview or plot summary of the movie
- `popularity`: Popularity score of the movie
- `poster_path`: URL of the movie's poster image
- `release_date`: Release date of the movie
- `title`: Title of the movie
- `video`: Whether the movie has video content (True or False)
- `vote_average`: Average vote rating for the movie
- `vote_count`: Total number of votes for the movie

## Data Processing

We use the following data fields for our prediction:
- `genre_ids`: Genre IDs associated with the movie (used as input features)
- `title`: Title of the movie (used for analysis)
- `overview`: Overview or plot summary of the movie (used for analysis)

## Predictive Model

We use logistic regression to predict movie genres based on the collected data. Logistic regression is a binary classification algorithm that can be used to predict whether a movie belongs to a particular genre or not.

## Colab Notebook

For a step-by-step implementation and detailed analysis, you can access the Colab notebook [here](https://colab.research.google.com/drive/1jCKiMV032zm8deE4rlK61pCzj8Hskmxz#scrollTo=8iDxrKBSsnDD).

Feel free to customize and extend this project for your own movie genre prediction tasks.
