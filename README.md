# NLP Based Cross Domain Movie Recommendation System


This study presents an innovative NLP-based cross-domain recommendation system that suggests movies based on the thematic and emotional essence of song lyrics. By leveraging advanced NLP techniques, the system bridges the gap between music and movies, providing personalized recommendations that resonate emotionally.

## Research Overview

The recommendation system uses the following NLP techniques:
- **Sentence-BERT:** For generating semantic embeddings of song lyrics and movie plots.
- **TextBlob:** For sentiment analysis to assess the emotional tone of lyrics and movie descriptions.
- **KeyBERT:** For extracting thematic keywords from both song lyrics and movie plots.

### Key Features
- **Cosine Similarity:** The core recommendation process involves calculating cosine similarity between song lyric embeddings and movie plot embeddings.
- **Sentiment Scores and Keywords:** The recommendations are enhanced by integrating sentiment polarity scores and thematic keywords from both domains, ensuring that the mood and storyline of the song align with the recommended movie.

## Datasets

The system uses datasets from the following sources:
- **Spotify & Genius:** For song lyrics and metadata (e.g., song title, artist).
- **OMDB API:** For movie details, including plot summaries, genres, and titles.
- **User Interaction Data (Optional):** This dataset can include feedback or user interactions for fine-tuning the recommendations.

## Repository Structure

Crossdomain_RS/
│
├── datasets/
│   ├── omdb_movie_dataset.xls
│   ├── SPOTIFY_GENIUS_SONG_DATASET.xls
│
├── notebooks/
│   ├── OMDB_MOVIE_DATASET_CREATION.ipynb
│   ├── Preprocessing_movies_dataset.ipynb
│   ├── Preprocessing_music_dataset.ipynb
│   ├── Recommendation_SBERT+EXTRACTED_KEYWORDS+SENTIMENT_SCORE.ipynb
│   ├── Recommendation_SBERT+EXTRACTED_KEYWORDS.ipynb
│   ├── Recommendation_SBERT+SENTIMENT_SCORE.ipynb
│   ├── Recommendation_SBERT.ipynb
│   ├── SPOTIFY_GENIUS_MUSIC_DATASET_CREATION.ipynb
│   ├── TF-IDF_for_Baseline_Comparision.ipynb
│
└── README.md



Crossdomain_RS/ │ ├── datasets/ │ ├── omdb_movie_dataset.xls # Movie dataset from OMDB API │ ├── SPOTIFY_GENIUS_SONG_DATASET.xls # Song dataset from Spotify and Genius APIs │ ├── notebooks/ │ ├── OMDB_MOVIE_DATASET_CREATION.ipynb # Dataset creation script for OMDB movie dataset │ ├── Preprocessing_movies_dataset.ipynb # Data preprocessing for movie dataset │ ├── Preprocessing_music_dataset.ipynb # Data preprocessing for song dataset │ ├── Recommendation_SBERT+EXTRACTED_KEYWORDS+SENTIMENT_SCORE.ipynb # Recommendation generation with SBERT, extracted keywords, and sentiment analysis │ ├── Recommendation_SBERT+EXTRACTED_KEYWORDS.ipynb # Recommendation generation with SBERT and extracted keywords │ ├── Recommendation_SBERT+SENTIMENT_SCORE.ipynb # Recommendation generation with SBERT and sentiment analysis │ ├── Recommendation_SBERT.ipynb # Basic recommendation generation with SBERT │ ├── SPOTIFY_GENIUS_MUSIC_DATASET_CREATION.ipynb # Dataset creation script for Spotify and Genius song dataset │ ├── TF-IDF_for_Baseline_Comparision.ipynb # TF-IDF based baseline comparison │ └── README.md # Project description and instructions
