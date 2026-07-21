# Movie Recommendation System

This project is a content-based movie recommendation system built using Python and machine learning techniques. Instead of recommending movies based on user ratings, it suggests similar movies by analyzing their content, such as genres, keywords, overview, cast, and crew.

The main goal of this project was to learn how recommendation systems work and implement one from scratch using text processing and similarity search.

---

## Dataset

The project uses the TMDB movie dataset, which contains information about thousands of movies.

The main datasets include:

- movies.csv
- credits.csv

After merging both datasets, the required features were selected for building the recommendation system.

---

## Project Workflow

The project follows these steps:

- Loaded the movie and credits datasets
- Merged both datasets using the movie ID
- Removed unnecessary columns
- Handled missing and duplicate values
- Extracted useful information from genres, keywords, cast, and crew
- Combined multiple text features into a single feature
- Applied text preprocessing
- Converted text into numerical vectors using TF-IDF
- Calculated similarity between movies
- Built a recommendation function
- Saved the processed data and model using Pickle

---

## Features Used

The recommendation model is mainly based on:

- Movie Overview
- Genres
- Keywords
- Cast
- Crew

These features are combined into a single text column before vectorization.

---

## Machine Learning Techniques

This project uses several NLP and machine learning techniques:

- TF-IDF Vectorization
- Cosine Similarity / Nearest Neighbors
- Text Preprocessing
- Feature Engineering

---

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Pickle
- Matplotlib

---

## Project Structure

```
Movie-Recommendation-System/
│
├── Movie_Recommendation.ipynb
├── movies.csv
├── credits.csv
├── movie_list.pkl
├── similarity.pkl
├── README.md
```

---

## How It Works

When a movie title is provided, the system:

1. Finds the selected movie.
2. Converts all movie descriptions into TF-IDF vectors.
3. Measures similarity between movies.
4. Returns the most similar movies based on their content.



## Future Improvements

Some improvements I plan to make in the future:

- Add a web interface using Flask or FastAPI
- Include movie posters using the TMDB API
- Improve recommendations with hybrid filtering
- Optimize the model for larger datasets

---

