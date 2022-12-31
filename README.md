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

## Data Visualization

![Screenshot 2022-12-31 113901](https://user-images.githubusercontent.com/78556152/210130723-efbdf2d1-c6c4-456c-be50-fb19a892c293.png)

From the above histograms, Kurtosis is positively skewed while Entropy is negatively skewed. Variance is multimodal, target is bimodal while skewness is random.

## Splitting Data and Training the Model

All independent variables are assigned to X while the dependent variable "Target" is assigned to y.

80% of the dataset is used for training and the remaining 20% for testing

Several classification algorithms including Logistic Regression, Naive Bayes, KNN and Support Vector Machine are used to train the model.

Each algorithm gives different results with different accuracy values as shown by classification report, accuracy report, F1 Score and Recall Score as shown below:

#### Logistic Regression

![Screenshot 2022-12-31 115031](https://user-images.githubusercontent.com/78556152/210130975-647dde8a-9e59-4ee7-b36c-c9a2959bfe49.png)

![Screenshot 2022-12-31 115226](https://user-images.githubusercontent.com/78556152/210131009-a6a4d304-5ebf-41a4-8f22-babb555f1ace.png)

#### KNN Algorithm

![Screenshot 2022-12-31 115624](https://user-images.githubusercontent.com/78556152/210131109-852ec52b-95f3-478f-b0b4-0db8a1d919f9.png)

![Screenshot 2022-12-31 115718](https://user-images.githubusercontent.com/78556152/210131134-d1900a07-92d6-42c5-845b-0626b6036b6c.png)

#### Naive Bayes Algorithm

![Screenshot 2022-12-31 120032](https://user-images.githubusercontent.com/78556152/210131197-ac55ecff-26fd-4478-b3e1-20ab4f2d60ea.png)

![Screenshot 2022-12-31 120139](https://user-images.githubusercontent.com/78556152/210131220-7b002a08-4086-47b4-97a3-5a906c075b8d.png)

#### Support Vector Machine Algorithm

![Screenshot 2022-12-31 120421](https://user-images.githubusercontent.com/78556152/210131277-a292e337-82aa-4c44-a808-0a893b0f5181.png)

![Screenshot 2022-12-31 120509](https://user-images.githubusercontent.com/78556152/210131300-3ccc38bb-9a87-400f-9b26-4b514a1f08cd.png)


## Comparing Between the Algorithms using F1 score and Recall

#### Algorithms F1 Score

![Screenshot 2022-12-31 121531](https://user-images.githubusercontent.com/78556152/210131557-cd95b7d3-6ba6-4d86-9be3-d35f93d532da.png)
