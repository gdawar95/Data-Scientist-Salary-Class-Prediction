# Data-Scientist-Salary-Class-Prediction

## Background:
Kaggle has hosted an open data scientist competition in 2019 titled “2019 Kaggle ML & DS Survey Challenge.” The purpose of this challenge was to “tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration.” More information on the competition, data, and prizes can be found on: https://www.kaggle.com/c/kaggle-survey-2019

The original data (multiple_choice_responses.csv) has been transformed to Kaggle_Salary.csv as per the code given in KaggleSalary_DataSet.ipynb. In the dataset to be used (Kaggle_Salary.csv- File to be read in notebook for this Project), rows with the null values of salaries have been dropped. In addition, two columns (‘Q10_Encoded’ and ‘Q10_buckets’) has been added at the end. Column ‘Q10_buckets’(Target Variable for Assignment 1) has been obtained by combining some salary buckets in the column ‘Q10’. Column ‘Q10_Encoded’ has been obtained by label encoding the column ‘Q10_buckets'.

## The purpose of this Project is to
1) understand and explore employment in the data science community, as represented in a survey conducted by Kaggle.
2) train, validate, and tune multi-class ordinary classification problem that can classify, given a set of survey responses by a data scientist, what a survey respondent’s current yearly compensation bucket is.

Classification is a supervised machine learning approach used to assign a discrete value of one variable when given the values of others. Many types of machine learning models can be used for training classification problems, such as logistic regression, decision trees, kNN, SVM, random forest, gradientboosted decision trees and neural networks.

## Contents of notebook
0. PREPARING NOTEBOOK
1. DATA PREPARATION
1.1    Check for missing value count
 
    1.1.1    Visualizing missing data using sns.heatmap
    1.1.2    Visualizing missing data using msno.matrix
    1.1.3    Checking missing values in each feature and inspecting the questions of the respective features
    1.1.4    Inspecting all the questions
 
1.2    Considering all features as performing imputation and one-hot encoding
 
    1.2.1    Now checking for the remaining features with missing values
    1.2.2    Checking which data to impute: mean, median or mode
    1.2.3    Checking Categorical Data
    1.2.4    Final inspection of missing data using a SNS and msno heatmaps
    
2. DATA EXPLORATION
2.1    Exploring - the profession of the responders and their cumulative frequency
 
2.2    Exploring the age group and sex ratio of the responders with thier response frequency
 
2.3    Exploring the Gender and Salary distribution of the responders with their response frequency
 
2.4    Box Plots for salary distribution
 
    2.4.1    Exploring Distribution of salary with age
    2.4.2    Exploring Distribution of salary with work experience
    2.4.3    Exploring Distribution of salary with Profession
    2.4.4    Exploring Distribution of salary with Country
    2.4.5    Exploring Distribution of salary with Amount spend on machine learning tools
    
3. FEATURE SELECTION
3.1    Converting categorical data into numbers
 
    3.1.1    Label Encoding Ordinal Data
    3.1.2    Encoding for Nominal Data
                - Correlation Matrix
                - Feature Selection by random forest (accepted)
                - Feature Selection by Lasso Regression (accepted)
    3.1.3    Performing Standard Scaling and PCA
    
4. MODEL IMPLIMENTATION
4.1    Finding the salary class probabilities on test data by implimenting ordinal logistic regression
 
4.2    Exploring the dataframe of salary class probabilities
 
4.3    Model Accuracy and Confusion Matrix
 
4.4    Cross validation for training and testing accuracy of the model over 10 folds of training data
 
4.5    Model Evaluation with Learning Curve (Bias Variance Tradeoff)

5. MODEL TUNING
5.1    Lasso-Feature-Selection Tuning
 
5.2    Multi-Class-Ordinal-Logistic-Regression Tuning

6. TESTING & DISCUSSION
6.1    Using the optimal model to make predictions on test set
 
6.2    Comparing the dataframe of salary class probabilities Tuned and Untuned
 
6.3    Comparing Model Accuracy and Confusion Matrix Tuned and Untuned
 
6.4    Cross validation for training and testing accuracy of the TUNED model over 10 folds
 
6.5    TUNED Model Evaluation with Learning Curve (Bias Variance Tradeoff)

7. CONCLUSION
