# Prudential Life Insurance Risk Prediction

This project has been done as part of the Applied Linear Algebra and Matrix Analysis Course at Northeastern University.

This project focuses on utilizing Principal Component Analysis (PCA) and Kernel Principal Component Analysis to improve the efficiency of processing time and reduce labor-intensive tasks for new and current clients of Prudential Life Insurance. The objective is to analyze risk factors and categorize clients based on their risk level. The dataset used in this project was obtained from a Kaggle search on Prudential Life Insurance.

## Techniques Used
### Principal Component Analysis (PCA)
PCA is a linear dimensionality reduction technique widely used in data preparation. It involves combining the original data linearly to reveal underlying patterns that may not be evident in the raw data. PCA helps in reducing the dimensions of the data while retaining most of the relevant information.

### Kernel Principal Component Analysis
Kernel PCA is an extension of PCA that addresses non-linearity in the data. By applying kernel functions, it allows for more complex data patterns to be captured, which may not be achievable through linear transformations alone.

## Data Description
The dataset used in this project consists of training and testing data. The training data contains 59,381 samples with 128 features, including an ordinal measure of risk with eight levels. The testing data has 19,765 samples without labels in the response variable.

## Data Pre-processing
The following steps were performed as part of the data pre-processing phase:

1. Checking Null Values: Missing values were identified in the dataset, and the percentage of missing values in each column was calculated.
2. Imputing Null Values: Columns with a null threshold above 40% were removed. For the remaining columns, missing values were imputed with either the mean or median, depending on the skewness of the data.
3. Removing Outliers: Outliers were removed from the dataset. Correlation analysis and feature score calculation using Mutual Independence (χ^2) were performed to identify the least important features for removal.
4. Normalizing Data: The remaining data was normalized before applying machine learning models.

## Machine Learning Models Used
The following machine learning models were trained using PCA and Kernel PCA on a 50-50 Train-Test split of the training dataset:

Logistic Regression
Linear Regression
Support Vector Classification
SGD Classifier
XGB Classifier
Random Forest Classifier
K-Neighbors Classifier
Artificial Neural Networks

## Results
The accuracy scores were achieved by each model using PCA and Kernel PCA.

## Conclusion
Principal Component Analysis (PCA) and Kernel Principal Component Analysis (Kernel PCA) were applied to Prudential Life Insurance data to predict risk levels. The comparison of PCA and Kernel PCA showed that PCA performed better in logistic regression and XGBoost Classifier.
