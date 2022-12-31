# Data-Science-2-Banknote-Authentication
A data science project for detecting fake bank notes

This project classifies banknotes in classes of genuine and fake notes.

A model is trained to detect fake notes from genuine notes.

The dataset used here is the banknote Authentication dataset from kaggle. This dataset contains features extracted from wavelet transformed images of both fake and genuine notes.

These features are

. Variance of the wavelet transformed image

. Skewness of the wavelet transformed image

. kurtosis of the wavelet transformed image

. entropy of the wavelet transformed image and 

. classes based on the above features


Several algorithms including Support Vector Machine, K-Nearest Neighbors, Naive Bayes and Logistic Regression are used to train the model for this project.

## Data

The data used for this project is "BankNoteAuthentication.csv" from kaggle.

## Preparing and Exploring Data

The dataset has 1372 rows and 5 columns. Each column represent the features extracted from banknote images of fake and genuine notes.

Variance, Skewness,	Kurtosis, and	Entropy are independent variables while class is the dependent variable. 

The independent variables provide features that differentiate between the two types of banknotes.

Class column represents the two classes of banknotes; class 0 representing genuine while class 1 representing fake notes.

The class column is renamed to "Target" for easy clarification. This is because the algorithm will give it as a predicted result.

Plotted figures are saved as png image files for future refrence.

There are no null values which makes it easy to fit the data to algorithms.

There are 24 duplicated values.

From the dataset, there are 762 genuine notes and 610 fake notes as shown below:

![Screenshot 2022-12-31 113030](https://user-images.githubusercontent.com/78556152/210130545-39e65cf6-caa0-4cab-881c-c4901bd6a24e.png)
