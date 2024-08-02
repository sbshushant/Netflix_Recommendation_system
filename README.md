# Netflix_Recommendation_system

Introduction
This project focuses on building a recommendation system using the Netflix dataset. The system uses Singular Value Decomposition (SVD) for making recommendations based on user ratings.

Table of Contents
Introduction About the Dataset Data Preprocessing Exploratory Data Analysis (EDA) Model Building Model Evaluation Recommendation System Conclusion

About the Dataset
The Netflix dataset used for this project contains information about user ratings for various movies. The key features include:

Cust_Id: Customer ID Rating: Rating given by the customer (1 to 5 stars) Movie_Id: Movie ID Year: Year of movie release Name: Name of the movie

Data Preprocessing
Loading Data:
The dataset was loaded into a pandas DataFrame for inspection.

Data Type Conversion:
Converted the Rating column to float type for numerical operations.

Handling Missing Values:
Identified and handled missing values in the dataset. Exploratory Data Analysis (EDA)

Rating Distribution:
Analyzed the distribution of ratings to understand user preferences. Plotted the count of each rating (1 to 5 stars).

Customer and Movie Counts:
Calculated the total number of unique customers and movies in the dataset. Determined the total number of ratings provided by customers.

Model Building
SVD Algorithm:
Implemented the Singular Value Decomposition (SVD) algorithm for matrix factorization. Used the surprise library to build the recommendation model.

Data Preparation:
Prepared the data for SVD by creating a dataset with customer IDs, movie IDs, and ratings. Limited the dataset to the top 100,000 rows for quicker runtime during model development.

Model Evaluation
Cross-Validation:
Evaluated the model using cross-validation with Root Mean Square Error (RMSE) and Mean Absolute Error (MAE) as metrics. Performed cross-validation with 3 folds.

Recommendation System
User-Specific Recommendations:
Selected a specific user (e.g., user ID 712664) to make movie recommendations based on their past ratings. Generated a list of movies the user has rated highly in the past.

Building the Recommendation Algorithm:
Created a copy of the movie titles dataset for manipulation. Trained the SVD algorithm on the entire dataset. Predicted the estimated score for each movie for the selected user. Sorted and displayed the top recommended movies for the user.

Conclusion
The analysis demonstrated the application of Singular Value Decomposition (SVD) for building a recommendation system using the Netflix dataset. Key findings include:

The SVD algorithm effectively handled the large dataset and provided accurate recommendations. The recommendation system generated personalized movie suggestions for users based on their past ratings. These insights highlight the utility of SVD in developing recommendation systems and its effectiveness in handling large-scale datasets with sparse ratings. This approach can be applied to various recommendation scenarios, such as movies, books, and products.
