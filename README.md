# Movie Rating Prediction with Python

## Project Overview

This project focuses on predicting IMDb movie ratings using a dataset of Indian films. By applying machine learning techniques, we aim to uncover the key factors that influence a movie's success and build a predictive model to estimate its rating. This analysis provides valuable insights for filmmakers, production houses, and movie enthusiasts.

## Objective

The primary objective is to develop a robust machine learning model that accurately predicts movie ratings based on features like genre, director, actors, and release year. We explore various regression algorithms and evaluate their performance to identify the most effective model for this task.

## Dataset

The dataset used in this project is the "IMDb Movies India" dataset, which contains information about Indian films. Key features include:

- **Name:** The title of the movie.
- **Year:** The year of release.
- **Duration:** The length of the movie in minutes.
- **Genre:** The genre(s) of the movie.
- **Rating:** The IMDb rating of the movie (our target variable).
- **Votes:** The number of votes received.
- **Director:** The director of the movie.
- **Actors:** The lead actors in the movie.

## Tools and Libraries

This project is developed in a Google Colab environment and utilizes the following Python libraries:

- **Pandas:** For data manipulation and analysis.
- **NumPy:** For numerical operations.
- **Matplotlib & Seaborn:** For data visualization.
- **Scikit-learn:** For machine learning tasks, including data preprocessing, model training, and evaluation.

## Methodology

1.  **Exploratory Data Analysis (EDA):** We began by analyzing the dataset to understand the distribution of movie ratings and the relationships between different features.
2.  **Data Preprocessing and Feature Engineering:** We handled missing values, converted categorical features into a machine-readable format using one-hot encoding, and cleaned the data to prepare it for modeling.
3.  **Model Building:** We trained and evaluated two regression models:
    *   **Linear Regression:** A baseline model to understand the linear relationships in the data.
    *   **Random Forest Regressor:** A more advanced model to capture non-linear patterns.
4.  **Model Evaluation:** We compared the models based on Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to determine the best-performing model.
5.  **Feature Importance:** We analyzed the feature importances from the Random Forest model to identify the most influential factors in predicting movie ratings.

## Results

The Random Forest Regressor significantly outperformed the Linear Regression model, indicating that the relationships between the features and movie ratings are complex and non-linear.

| Metric | Linear Regression | Random Forest Regressor |
| :--- | :--- | :--- |
| **Mean Absolute Error (MAE)** | 1.91 | **0.91** |
| **Root Mean Squared Error (RMSE)** | 2.72 | **1.19** |

## Key Insights

- **Top Predictors:** The most important features for predicting movie ratings were the **Year** of release and the **Duration** of the movie.
- **Genre Influence:** Genre plays a significant role, with certain genres like 'Documentary' having a strong positive correlation with higher ratings.
- **Actor and Director Impact:** The model identified specific actors and directors who are associated with higher-rated films.

## Challenges Faced

- **Data Quality:** The dataset contained a significant number of missing values, which required careful handling.
- **High Cardinality of Categorical Features:** The 'Genre', 'Director', and 'Actor' columns had a large number of unique values, which made one-hot encoding challenging.
- **Non-Linear Relationships:** The poor performance of the Linear Regression model highlighted the non-linear nature of the data, which required a more complex model like Random Forest.

## Conclusion

This project successfully demonstrates the application of machine learning to predict movie ratings. The Random Forest model provides a reliable and accurate method for this task, offering valuable insights into the factors that drive a movie's success.
