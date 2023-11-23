# Movie Recommendation System with Sentiment Analysis

The Movie Recommendation System with Sentiment Analysis is a content-based recommender system that suggests movies similar to the ones a user likes. Additionally, it incorporates sentiment analysis on user reviews to enhance the recommendation process.

> **Note:** The application has been updated to a newer version. Access the source code of the latest version [here](https://github.com/bwambale03/MovieRec).

![GIF](./static/mrswsa.gif)

## Overview

Movie details such as title, genre, runtime, rating, poster, etc., are fetched using an API provided by TMDB (The Movie Database): [TMDB API Documentation](https://www.themoviedb.org/documentation/api). For sentiment analysis, user reviews from the IMDb site are extracted using `beautifulsoup4` after obtaining the IMDb ID from the TMDB API.

## How to Obtain an API Key?

1. Create an account on [TMDB](https://www.themoviedb.org/).
2. In your account settings, click on the `API` link from the left-hand sidebar.
3. Fill in all the required details to apply for an API key.
4. Once your request is approved, you can find the API key in the `API` sidebar.

## How to Run the Project?

1. Install all the required libraries mentioned in the [requirements.txt](https://github.com/kishan0725/Movie-Recommendation-System-with-Sentiment-Analysis/blob/master/requirements.txt) file.
   > **Note:** Consider downgrading the resources in the `requirements.txt` file as the models were trained using specific versions. Adjust the models to suit the latest versions on your machine.

2. Clone this repository to your local system.
3. Replace `YOUR_API_KEY` in the `main.py` file with your TMDB API key.
4. Open the command prompt from your project directory and run the command `python main.py`.
5. Open your browser and navigate to `http://127.0.0.1:5000/`.
6. You are done!

## Similarity Score:

How does the system determine which item is most similar to the one the user likes? The similarity score plays a crucial role. This numerical value ranges from zero to one and helps quantify how similar two items are on a scale from zero to one. The similarity score is obtained by measuring the similarity between the text details of two items, and it is often calculated using cosine-similarity.

## Sources of the Datasets:

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of Movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of Movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of Movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
