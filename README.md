# Movie Recommendation System
## Project Overview
This project implements a movie recommendation system based on movie metadata. The system uses a content-based filtering approach to suggest movies that are similar to a given movie.

## Data Source
The dataset used for this project is imdb_movies.csv. This dataset contains information about movies, including names, scores, genres, overviews, crew, and other relevant details.

## Methodology
The recommendation system is built using the following steps:

### Data Loading and Initial Exploration: 
The imdb_movies.csv dataset is loaded into a pandas DataFrame. Initial checks are performed to understand the data structure, size, and identify potential issues like duplicate entries and missing values.

### Data Preprocessing:

Duplicate entries based on the original title (orig_title) are identified and removed.

Missing values in the 'genre' and 'crew' columns are handled by dropping rows with missing data in these specific columns.

The 'date_x' column is converted to datetime objects, and new columns for 'Release_year' and 'Release_Month' are extracted.

### Feature Engineering:
Relevant text features such as 'genre', 'overview', and 'crew' are likely combined or processed to create a representation of each movie's content. (Based on the use of TfidfVectorizer and cosine_similarity, it's inferred that a text-based similarity approach is used).

### Similarity Calculation: 
TF-IDF (Term Frequency-Inverse Document Frequency) is used to vectorize the text features. Cosine similarity is then calculated between the TF-IDF vectors of all movies to determine their similarity scores.

### Recommendation Function:
A function is created to take a movie name as input and return a list of recommended movies based on the calculated cosine similarity scores.

## Technologies Used
Python

Pandas

NumPy

Scikit-learn (for TfidfVectorizer and cosine_similarity)

Seaborn

Matplotlib

## How to Run
Clone this repository to your local machine.

Ensure you have Python and the required libraries (pandas, numpy, scikit-learn, seaborn, matplotlib) installed.

Make sure the imdb_movies.csv dataset is in the same directory as the notebook.

Run the MovieRecommendationSystem.ipynb Jupyter Notebook in a compatible environment (like Jupyter Notebook, JupyterLab, or VS Code).

## Future Work
Explore different feature combinations and weighting for improved recommendations.

Implement other recommendation techniques (e.g., collaborative filtering).

Build a user interface for the recommendation system.

Evaluate the performance of the recommendation system using appropriate metrics.
