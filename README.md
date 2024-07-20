# Movie-Recommendation-System

**Special Thanks (CampusX -- Youtube Channel) for this learning**
**Special Thanks to SOURAV SAHOO for the DataSet**
**DataSet Link **https://www.kaggle.com/datasets/souravdatascience/tmdb-5000-movies-details**** 

**Overview**
This project implements a movie recommendation system using content-based filtering. The system suggests movies based on the similarities between the tags of movies, which include genres, keywords, cast, crew, and overview.

**Features**
**Data Preprocessing:**
Merges movie metadata and credit information.
Converts JSON-like strings in columns to lists.
Extracts genres, keywords, cast, and crew information.
Cleans and processes text data (e.g., removing spaces, stemming).

**Feature Extraction:**
Uses CountVectorizer to convert text data into numerical vectors.
Applies stemming to reduce words to their root forms.

**Similarity Calculation:**
Computes cosine similarity between movies based on their tags.

**Recommendation System:**
Recommends movies similar to the selected movie based on the computed similarities.

**User Interface:**
A web interface created using Streamlit allows users to select a movie and get recommendations.
Files Included
tmdb_5000_movies.csv: Movie metadata file.
tmdb_5000_credits.csv: Movie credits file.
movies_dict.pkl: Pickle file containing movie data.
similarity.pkl: Pickle file containing similarity matrix.
app.py: Streamlit application file for the recommender system.

**Setup**
**Install Required Libraries:**

Ensure you have the following Python libraries installed:
pandas
numpy
sklearn
nltk
streamlit
pickle (usually comes with Python standard library)

**How It Works**

**Data Loading and Merging:**
Loads the movies and credits datasets.
Merges them on the movie title to create a comprehensive dataset.

**Data Transformation:**
Converts genre, keyword, cast, and crew columns from JSON format to lists.
Cleans and preprocesses text data for feature extraction.

**Feature Extraction and Similarity Calculation:**
Extracts features using CountVectorizer.
Computes the cosine similarity between movie vectors.

**Recommendation Generation:**
Finds similar movies based on the cosine similarity matrix.
Returns a list of recommended movies.

**Streamlit Interface:**
Provides a user-friendly interface to interact with the recommender system.
