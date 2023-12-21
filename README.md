# FakeNewsPrediction

This Python code performs text classification using a logistic regression model on a dataset of news articles. Here is a description of the code:

    Importing Libraries:
        The code starts by importing necessary libraries, including NumPy, Pandas, regular expression (re), Natural Language Toolkit (nltk), and scikit-learn modules.

    Data Preprocessing:
        Downloads the English stop words from NLTK.
        Reads a CSV file containing a dataset of news articles using Pandas.
        Checks for and fills any missing values in the dataset.

    Text Preprocessing:
        Combines the 'author' and 'title' columns into a new 'content' column.
        Performs text preprocessing on the 'content' column, including:
            Converting text to lowercase.
            Removing non-alphabetic characters.
            Tokenizing the text.
            Applying stemming using the Porter Stemmer.
            Removing stop words.

    Feature Extraction:
        Uses TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to convert the processed text data into numerical vectors.

    Splitting Data:
        Splits the dataset into training and testing sets using scikit-learn's train_test_split function.

    Logistic Regression Model:
        Initializes a logistic regression model using scikit-learn's LogisticRegression.
        Fits the model to the training data.

    Model Evaluation:
        Predicts labels for both the training and testing sets.
        Calculates and prints the accuracy scores for both the training and testing predictions using scikit-learn's accuracy_score function.

    Prediction and Analysis:
        Applies the trained model to a new set of data (X_new) and prints the predictions.
        Counts and prints the occurrences of predicted labels and true labels in the testing set.

The overall goal of the code is to preprocess a dataset of news articles, train a logistic regression model on the processed text data, and evaluate the model's performance on both training and testing sets. The final part analyzes the distribution of predicted labels and compares them to the true labels in the testing set.
