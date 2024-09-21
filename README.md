# Heart Disease Prediction Using Machine Learning

## Overview
This project is aimed at predicting heart disease using machine learning techniques. The project involves the use of a Kaggle dataset with various medical and behavioral features, and applies multiple machine learning models to predict whether an individual is likely to suffer from heart disease.

## Project Structure

- **Dataset**: The dataset used for this project contains 50,000 data points with 17 features such as BMI, Smoking habits, PhysicalHealth, AgeCategory, etc. The target variable is `HeartDisease`, which indicates whether a person has heart disease or not.
  
- **Models Used**:
  1. K-Nearest Neighbors (KNN)
  2. Logistic Regression
  3. Support Vector Machine (SVM)

- **Results**: The SVM model achieved the highest accuracy and precision, making it the most reliable model for this dataset.

## Motivation
Heart disease is a leading cause of death globally, making early prediction and prevention essential. Machine learning models can assist in early diagnosis and help medical professionals in decision-making by analyzing patients' medical history and behavior.

## Dataset
The dataset was sourced from Kaggle and contains the following features:
- **Numerical Features**: BMI, PhysicalHealth, MentalHealth, SleepTime, etc.
- **Categorical Features**: Smoking, AlcoholDrinking, Stroke, etc.
  
The dataset is biased, with an uneven distribution of people with and without heart disease, which was handled using a random oversampler.

## Data Preprocessing
1. **Handling Null Values**: Rows with null values were dropped.
2. **Encoding**: Categorical values were encoded using an Ordinal Encoder.
3. **Feature Scaling**: MinMaxScaler was applied to ensure that features are within a normalized range of [0, 1].
4. **Dataset Splitting**: The dataset was split into training and testing sets in an 80:20 ratio using random splitting.

## Machine Learning Models
1. **K-Nearest Neighbors (KNN)**
2. **Logistic Regression**
3. **Support Vector Machine (SVM)**

### Model Evaluation
- **Accuracy**: The SVM model had the highest accuracy, followed by Logistic Regression.
- **Precision**: SVM had the highest precision.
- **Recall**: KNN had the highest recall, but with a higher error rate compared to SVM.

## Results
- **Confusion Matrix**: A confusion matrix was used to show the prediction errors of each model.
- **Error Analysis**: The KNN model had the highest error rate, while SVM had the lowest.

### ROC Curve
ROC curves for all models were plotted to visualize their performance.

## Conclusion
The Support Vector Machine (SVM) model outperformed others with the highest accuracy and precision. This machine learning model can be a useful tool in predicting heart disease, assisting in early diagnosis and prevention.

## Future Work
Improvements could be made by using larger and more diverse datasets. Additionally, tuning model parameters and trying other machine learning models like Neural Networks could further improve accuracy and precision.
