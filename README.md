# 🎬 Movie Recommendation System

## 📌 Project Overview

This project builds a content-based movie recommendation system using Python. The system recommends movies to users based on their similarity to a selected movie, using key content features like genres, keywords, and overview.

## 🎯 Objective

The goal of this project is to implement a recommendation engine that helps users discover movies they might enjoy, using metadata-based similarity measures.

## 🧪 Techniques Used

- **Content-Based Filtering**
- **Natural Language Processing (NLP)**
- **Cosine Similarity**
- **TF-IDF Vectorization**
- **Count Vectorizer**

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

## 🚀 How to Run

1. Clone this repository or download the notebook.
2. Install the required dependencies.
3. Launch Jupyter Notebook or JupyterLab.
4. Open `Movie_Recommendation_System.ipynb`.
5. Run all cells.
6. Use the function `recommend('Movie Title')` to get movie suggestions.

## 💻 Dependencies

Install the necessary libraries using:
