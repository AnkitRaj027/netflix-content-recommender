# 🎬 Netflix Content Recommendation System

A content-based recommendation system that suggests Netflix titles based on similarities in genres, descriptions, cast, directors, country, and content type.

## Overview

This project uses Natural Language Processing (NLP) and machine learning techniques to identify titles with similar content. It includes a baseline TF-IDF model, an improved weighted-feature model, evaluation experiments, and an interactive interface built in Google Colab.

## Features

- **Data preprocessing:** Handles missing values and prepares Netflix metadata.
- **TF-IDF vectorization:** Converts textual metadata into numerical representations.
- **Cosine similarity:** Ranks titles based on content similarity.
- **Weighted feature model:** Assigns different importance to genres, descriptions, cast, directors, type, and country.
- **Model comparison:** Compares baseline and improved recommendations.
- **Interactive interface:** Search for titles, select a model, and view recommendations.

## Tech Stack

- Python
- Pandas and NumPy
- Scikit-learn
- SciPy
- Matplotlib
- IPywidgets
- Google Colab

## How It Works

1. Load and clean the Netflix titles dataset.
2. Prepare text features from the available metadata.
3. Generate TF-IDF vectors for individual features.
4. Apply feature weights and combine the sparse matrices.
5. Calculate cosine similarity between titles.
6. Rank and display the top recommendations.

## Dataset

The project uses the Netflix Movies and TV Shows dataset available on Kaggle:

https://www.kaggle.com/datasets/shivamb/netflix-shows

Download `netflix_titles.csv` and upload it to your Colab session before running the notebook.

## How to Run

1. Open `netflix_content_recommender.ipynb` in Google Colab.
2. Download the dataset from Kaggle.
3. Upload `netflix_titles.csv` when prompted.
4. Run the notebook cells in order.
5. Use the interactive interface to explore recommendations.

## Evaluation

The project compares baseline and weighted-feature recommendations using genre overlap as a simple evaluation proxy. This metric measures shared categories, not actual user satisfaction.

## Future Improvements

- Add recommendation explanations.
- Handle duplicate titles more precisely.
- Tune feature weights using stronger evaluation methods.
- Deploy the interface as a standalone web application.

## Author

Developed as a machine learning project to explore content-based recommendation systems, text vectorization, similarity search, and interactive ML applications.
