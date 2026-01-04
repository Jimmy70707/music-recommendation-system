# Music Recommendation System 🎵

A content-based music recommendation system that suggests similar songs using Natural Language Processing (NLP), TF-IDF vectorization, and cosine similarity.  
The system is deployed as an interactive web application using Streamlit.

---

## Overview

Music discovery platforms often rely on user behavior or popularity-based algorithms.  
This project focuses on **content-based recommendation**, where songs are recommended based on lyrical similarity rather than user history.

The system analyzes song lyrics, converts them into numerical representations using TF-IDF, and computes similarity scores to recommend relevant tracks.

---

## Problem Statement

Finding musically similar songs based on lyrical content is challenging due to unstructured text data.  
Traditional rule-based approaches fail to capture semantic similarity effectively.

This project aims to solve this problem using NLP techniques and similarity metrics to provide meaningful music recommendations.

---

## Solution Approach

- Clean and preprocess song lyrics using NLP techniques
- Remove stopwords and special characters
- Convert text into TF-IDF vectors
- Compute cosine similarity between songs
- Recommend top similar songs based on similarity score
- Deploy the recommendation system using Streamlit

---

## Features

- Content-based song recommendation
- NLP-driven lyric analysis
- Fast similarity search using cosine similarity
- Interactive Streamlit web interface
- Logging for preprocessing and recommendation steps

---

## Tech Stack

- **Python**
- **Pandas**
- **NLTK**
- **Scikit-learn**
- **Streamlit**
- **Joblib**

---

## Project Structure

│music-recommendation-system/

├── preprocess.py # Data cleaning, NLP preprocessing, TF-IDF, similarity matrix

├── recommend.py # Recommendation logic

├── main.py # Streamlit web application

├── app.ipynb # Data analysis, visualization, and preprocessing notebook

├── requirements.txt # Project dependencies


---

## How It Works

1. Song lyrics are cleaned and tokenized.
2. Text is transformed into TF-IDF vectors.
3. Cosine similarity is calculated between all songs.
4. Given a selected song, the system finds the most similar songs.
5. Results are displayed in a clean table via Streamlit.

---

## How to Run the Project

1. Clone the repository:
```bash
git clone https://github.com/jimmy70707/music-recommendation-system.git
cd music-recommendation-system
1.Install dependencies:

pip install -r requirements.txt
2.Run preprocessing (only once):

python preprocess.py

3.Run recommend file

python recommend.py

4.Start the Streamlit app:

streamlit run main.py
```
Input
---
Selected song title from the dataset

Output
---
Top recommended songs based on lyrical similarity

Future Improvements
---
Optimize similarity computation for large datasets

Add song preview integration (Spotify / YouTube)

Use word embeddings (Word2Vec / BERT)

Improve UI with filters and recommendations score

Author
---
Mohamed Gamal

Machine Learning & AI Engineer

