# Movie Recommendation and Netflix Content Exploratory Data Analysis
## Project Overview
This project performs an exploratory data analysis (EDA) on a dataset of Netflix movies and TV shows. The goal is to understand the characteristics of the content available on Netflix, including the distribution of content types, ratings, and popular directors.

## Data Source
The dataset used for this analysis is netflix_titles.csv, which contains information about movies and TV shows available on Netflix.
Link to the dataset -> https://www.kaggle.com/datasets/ashpalsingh1525/imdb-movies-dataset

## Methodology
The analysis follows these steps:

### Data Loading: 
The dataset is loaded into a pandas DataFrame.

### Data Preprocessing:

Checked for missing values.

Filled missing values in the 'duration', 'rating', and 'date_added' columns with their respective modes.

Converted the 'date_added' column to datetime objects.

### Exploratory Data Analysis (EDA):

Analyzed the distribution of content types (Movie vs. TV Show) using value counts and a pie chart.

Examined the distribution of ratings using value counts and a bar plot.

Identified and listed the top 10 directors based on the number of movies/TV shows they have directed in the dataset.

## Key Findings
The dataset contains 8807 entries.

A significant portion of the content on Netflix is Movies.

The most common content ratings are TV-MA, TV-14, TV-PG, R, and PG-13.

The top directors in this dataset include Rajiv Chilaka, Raúl Campos, Jan Suter, Marcus Raboy, Suhas Kadav, Jay Karas, Cathy Garcia-Molina, Martin Scorsese, Youssef Chahine, Jay Chapman, and Steven Spielberg.

## Technologies Used
Python

Pandas

NumPy

Seaborn

Matplotlib

## How to Run
Clone this repository to your local machine.

Ensure you have Python and the required libraries (pandas, numpy, seaborn, matplotlib) installed.

Run the Final .ipynb Jupyter Notebook in a compatible environment (like Jupyter Notebook, JupyterLab, or VS Code).

## Future Work
Further analysis of genres and their popularity.

Investigating the relationship between release year and content added date.

Analyzing cast popularity.

Building a recommendation system based on content similarity.

