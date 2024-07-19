# Analysis of Consumer Behaviour to New Products

## Introduction

This project aims to develop a machine learning model to predict consumer behavior towards new products with at least 75% accuracy.

## Goal

The primary objective is to create a model that can predict customer behavior with a minimum accuracy of 75% using machine learning techniques.

## Stages

The project is divided into the following stages:

1. **Open the Data File**: Study its general information.
2. **Prepare the Data**: Clean and preprocess the data for analysis.
3. **Explore the Data**: Check for anomalies and patterns.
4. **Data Splitting**: Divide the data into three categories:
   - Training Set
   - Validation Set
   - Test Set
5. **Model Training and Tuning**:
   - Evaluate model quality by adjusting hyperparameters.
   - Test the model using the test set.
6. **Sanity Check**: Perform a final evaluation to ensure robustness.
7. **Draw Conclusions**: Summarize findings and model performance.

## Data Content

The dataset includes the following columns related to customer behavior:

- `calls`: Number of calls made.
- `minutes`: Total call duration in minutes.
- `messages`: Number of text messages sent.
- `mb_used`: Internet usage traffic in MB.
- `is_ultimate`: Package for the current month (1 for Ultimate, 0 for Surf).

## Conclusion

The goal of the project is to identify a model that achieves at least 75% accuracy in predicting consumer behavior towards new products. The data was split as follows:

- 60% for the training set
- 20% for the test set
- 20% for the validation set

Three types of models were evaluated:

1. **Logistic Regression**: Accuracy of 73.5%
2. **Decision Tree**: Accuracy of 71.6%
3. **Random Forest**: Accuracy of 78.2%

Among the models tested, the Random Forest Model demonstrated the highest accuracy. After tuning hyperparameters with the following settings:

- `n_estimators=2000`
- `criterion='gini'`
- `max_depth=5`

The accuracy improved to 78.3%. The sanity check was performed with a margin of error of 0.461.
