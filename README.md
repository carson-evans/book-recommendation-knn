# Book Recommendation System

## Project Overview

This project develops a book recommendation system using the Book-Crossings dataset. It utilizes Python, Pandas for data manipulation, Scipy for sparse matrix handling, and Scikit-learn for applying the Nearest Neighbors algorithm. The goal is to recommend books based on user ratings, showcasing collaborative filtering techniques in recommendation systems.

## Dataset

The dataset, sourced from the Book-Crossings community, includes:

- `BX-Books.csv`: Contains book details such as ISBN, book title, and author.
- `BX-Book-Ratings.csv`: Comprises user ratings for various books.

Initial preprocessing steps include merging the datasets, filtering out users who have rated fewer than 200 books, and books with fewer than 100 ratings to ensure data quality and relevance.

## Methodology

The recommendation system is built using the following steps:

1. **Data Preprocessing**: Importing the data, merging book titles with their corresponding ratings, and filtering the data to include only users and books with a significant number of ratings to ensure reliable recommendations.
2. **Data Visualization**: Plotting control histograms to observe the distribution of ratings among users and books.
3. **Matrix Transformation**: Converting the user-book ratings into a pivot table, thereby creating a sparse matrix suitable for fitting with the Nearest Neighbors model.
4. **Model Training**: Utilizing the Nearest Neighbors algorithm with cosine similarity to train the model on users' book ratings.
5. **Recommendation Function**: Implementing a function to recommend books based on a given book title by identifying the nearest neighbors (i.e., similar user ratings).

## Results

The recommendation system successfully suggests books that are similar to a given book based on user ratings. For example, recommending books related to "Where the Heart Is (Oprah's Book Club (Paperback))" yields titles such as "I'll Be Seeing You", "The Weight of Water", and "The Surgeon", among others, demonstrating the system's ability to identify and recommend books with similar reader appeal.

## Conclusion and Future Work

This project demonstrates the applicability of the Nearest Neighbors algorithm in building a simple yet effective book recommendation system. Future improvements could include exploring different similarity metrics, incorporating user feedback for dynamic updating of recommendations, or extending the system to incorporate content-based filtering techniques for a hybrid recommendation approach.
