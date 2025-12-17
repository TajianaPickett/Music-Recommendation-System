# Music Recommendation System (Spotify Audio Features)
## Project Overview
This project builds a **content-based music recommendation system** using Spotify audio features.  
Songs are recommended based on **sound similarity** rather than popularity or user behavior, making the system interpretable and data-driven.

## What This Project Taught Me
- **content-based recommender**
- feature scaling
- **PCA and t-SNE** to interpret high-dimensional data
- large, real-world datasets
- Balanced **model performance, interpretability, and practicality**

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn (KMeans, PCA, t-SNE)
- Plotly, Matplotlib, Seaborn
- Spotify Web API (Spotipy)

## Dataset
The project uses Spotify datasets containing:
- **170,000+ songs**
- Audio features including:
  - Danceability, energy, valence
  - Acousticness, instrumentalness, loudness
  - Tempo, speechiness, popularity

## Methodology

### Analysis
- Analyzed feature correlations with song popularity
- Examined trends in musical characteristics across decades
- Compared audio profiles of popular genres

### Clustering
- Applied **K-Means clustering** to:
  - Genres (10 clusters)
  - Songs (20 clusters)
- Standardized features using pipelines
- Visualized clusters using **PCA** and **t-SNE**

### Recommendation Engine
1. User inputs one or more songs (name + year)
2. Audio feature vectors are averaged
3. Songs are compared using **cosine similarity**
4. Closest matches are returned as recommendations

Spotify’s API (Spotipy) is used to retrieve missing track features when needed.

---

## Example

**Input**
- Come As You Are (1991)
- Smells Like Teen Spirit (1991)

**Recommended Songs**
- Otherside – Red Hot Chili Peppers
- Hanging By A Moment – Lifehouse
- No Excuses – Alice In Chains

## Key Takeaways
- Audio features are effective for modeling music similarity
- Clustering reveals structure across genres and listening styles
- Interpretable, feature-based recommenders can perform well without deep learning
