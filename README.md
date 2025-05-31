# 🎬 Movie Recommendation System

## 📌 Project Overview

This project builds a content-based movie recommendation system using Python. The system recommends movies to users based on their similarity to a selected movie, using key content features like genres, keywords, and overview.

## 🎯 Objective

The goal of this project is to implement a recommendation engine that helps users discover movies they might enjoy, using metadata-based similarity measures.

## 📊 Dataset

- **Source:** The Movies Dataset (also available on Kaggle)
- **Key Columns Used:**
  - `title`
  - `genres`
  - `keywords`
  - `overview`
  - `cast`, `crew`, `director`

## 🛠️ Features

- Extracts and cleans metadata like genres, keywords, and cast.
- Combines textual features into a single string representation.
- Uses vectorization (TF-IDF or CountVectorizer) and cosine similarity to find similar movies.
- Takes a movie title as input and returns a list of top N recommended titles.

## 🧪 Techniques Used

### Method 1:
Collaborative Filtering is a technique that recommends movies based on the preferences of similar users. 
1.	Converting Data into a Sparse Matrix since lot of values are 0’s. 
2.	A KNN model is used to find similar movies based on user rating patterns. The similarity between movies is measured using cosine similarity.
3.	Created a recommendation function.
4.	Using Gradio created small app for user interaction.

### Method 2:
Content-based filtering recommends movies that are similar in content (e.g., genre). Instead of looking at user ratings, it compares the attributes of the movies. 
The genres column contains multiple genres separated by |. To process this:
•	Genres were split into a list for each movie.
•	One-hot encoding was applied to convert genres into numerical features.
A cosine similarity matrix was created to compute similarity scores between movies based on genres.


## 🚀 How to Run

1. Clone this repository or download the notebook.
2. Install the required dependencies.
3. Launch Jupyter Notebook or JupyterLab.
4. Open `Movie_Recommendation_System.ipynb`.
5. Run all cells.
6. Use the function `recommend('Movie Title')` to get movie suggestions.

