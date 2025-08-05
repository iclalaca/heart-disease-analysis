# Heart Disease Prediction using Machine Learning

This project focuses on predicting the presence of heart disease using clinical data from the [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction). Two supervised machine learning algorithms—**K-Nearest Neighbors (KNN)** and **Random Forest**—were implemented and evaluated to classify whether a patient is likely to develop heart disease.

## 📌 Objectives

- Clean and preprocess the dataset  
- Perform exploratory data analysis and visualizations  
- Train and evaluate KNN and Random Forest models  
- Perform hyperparameter tuning with **GridSearchCV**  
- Identify and visualize the most important features  

---

## 📊 Visualizations

A range of data visualizations were created to better understand the dataset:

- **Bar Chart**: Distribution of the target classes  
- **Heatmap**: Correlation between features  
- **ROC Curves + AUC Scores**: Model performance comparison  
- **Confusion Matrices**: Evaluation of classification accuracy  
- **Feature Importance Plot**: Most influential clinical factors in heart disease prediction  

---

## 🧹 Data Preprocessing

- Removed or treated missing and outlier values  
- Normalized numerical features where necessary  
- Categorical encoding (if applicable)  
- Target class balance was examined  

---

## ⚙️ Machine Learning Models

### 1. K-Nearest Neighbors (KNN)
- Tuned using `GridSearchCV`
- Best parameters:
  - `metric='manhattan'`
  - `n_neighbors=15`
  - `weights='distance'`

### 2. Random Forest Classifier
- Provided the best results in terms of accuracy and robustness  
- Also used for calculating **feature importances**

---

## 🔍 Feature Importance

The following features were identified as most influential in predicting heart disease:

1. **ST_Slope**  
2. **MaxHR** (Maximum Heart Rate)  
3. **ExerciseAngina**  

---

## ✅ Results

| Model            | Accuracy (Cross-Validated) | Notes                          |
|------------------|-----------------------------|-------------------------------|
| KNN              | 0.713178  | Tuned with GridSearchCV       |
| Random Forest    | 0.860465  | Best performing model overall |

---

## 🛠️ Tech Stack

- Python  
- scikit-learn  
- pandas  
- matplotlib  
- seaborn  
- NumPy  
