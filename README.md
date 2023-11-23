# Movie Recommendation System With sentiment_analysis

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

<blockquote>
   <b>Note</b>: The application has been updated to a newer version. Get the source code of the newer version <a href="https://github.com/bwambale03/MovieRec">here</a>
</blockquote>

![GIF](./static/mrswsa.gif)

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using `beautifulsoup4` and performed sentiment analysis on those reviews.

## How to get the API key?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. You will see the API key in your `API` sidebar once your request is approved.

## How to run the project?

1. Install all the libraries mentioned in the [req'ts.txt](https://github.com/kishan0725/Movie-Recommendation-System-with-Sentiment-Analysis/blob/master/requirements.txt) file. 
## NB
# consider downgrading the resources in req'ts.txt file since the models used here were trained using these specific versions. consider refining the models to suite the latest versions on your machine
2. Clone this repository in your local system.
3. Replace YOUR_API_KEY in the `main.py` file.
4. Open the command prompt from your project directory and run the command `python main.py`.
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
6.Done
## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here we use the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

