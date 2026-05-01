# Spam Detection Project:

This project aims to build a spam detection model using the Multinomial Naive Bayes algorithm. The dataset used contains SMS messages labeled as either 'spam' or 'ham'.

## Project Process:

1.  **Data Loading and Exploration**: The SMS spam dataset was loaded into a pandas DataFrame. Initial data exploration included checking the shape of the dataset, column names, missing values, and duplicate entries.
2.  **Data Cleaning**: Duplicate entries were removed from the dataset. A text cleaning function was applied to the 'Message' column to convert text to lowercase, remove special characters and numbers, and strip leading/trailing spaces.
3.  **Data Visualization**: Pie and count plots were generated to visualize the distribution of 'spam' and 'ham' messages in the dataset.
4.  **Data Preparation**: The 'Category' column was mapped to numerical values (0 for 'ham' and 1 for 'spam'). The 'Message' column was transformed into a matrix of token counts using `CountVectorizer`.
5.  **Model Training**: The data was split into training and testing sets. A Multinomial Naive Bayes model was initialized and trained on the training data.
6.  **Model Evaluation**: The trained model was evaluated on both the training and testing data using accuracy score, classification report, and confusion matrix.
    - Accuracy on training data: 0.9915
    - Accuracy on testing data: 0.9680
