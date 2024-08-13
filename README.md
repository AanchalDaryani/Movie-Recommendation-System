# Movie Recommendation System

## Overview
This project is a movie recommendation system that suggests similar movies based on a user's favorite movie. The system utilizes TF-IDF vectorization and cosine similarity to analyze the relationships between movies and provide recommendations.

## Features
- **Input:** User can enter the name of their favorite movie.
- **Output:** The system returns a list of recommended movies that are similar to the input movie.
- **Similarity Analysis:** Utilizes cosine similarity to measure the similarity between movies based on selected features such as genres, keywords, tagline, cast, and director.

## Dataset
The dataset used in this project contains information about various movies, including:
- Title
- Genres
- Keywords
- Tagline
- Cast
- Director

The dataset consists of 4,803 movies with 24 features.

## Getting Started
To run this project, ensure you have the necessary libraries installed. You can install them using pip:

```bash
pip install pandas scikit-learn numpy difflib
```

### Usage
1. **Load the Dataset:** Import the movies dataset into a DataFrame.
2. **Data Preprocessing:**
   - Replace null values in selected features with empty strings.
   - Combine selected features into a single string for each movie.
3. **Vectorization:**
   - Convert the combined feature strings into feature vectors using TF-IDF.
4. **Cosine Similarity:**
   - Calculate the cosine similarity between the feature vectors to identify similar movies.
5. **Get Recommendations:**
   - Prompt the user to input their favorite movie name.
   - Find the closest match in the dataset.
   - Retrieve and display the top recommended movies based on similarity scores.

### Example
```python
movie_name = input('Enter your favourite movie name: ')
```

## Conclusion
This movie recommendation system efficiently suggests 30 similar movies using TF-IDF and cosine similarity techniques. It provides users with personalized movie suggestions, enhancing their viewing experience by helping them discover new films based on their interests.


