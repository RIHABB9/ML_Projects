# Calories Burnt Prediction

## 🎯 Objective
Build a regression-based machine learning model to predict the number of calories burnt during exercise, using biological measures.

## 📊 Dataset
- Calories dataset (calories.csv)
- Exercise dataset (exercise.csv)
  
Merged into a single dataframe containing attributes (such as Age, Height, Weight, Gender, Exercise Duration, Heart Rate, Body Temperature) and the target variable Calories.

## 🔑 Key Steps
1. Data cleaning and merging of the two datasets
2. Exploratory analysis (scatter plots, distribution plot, correlations)
3. Feature encoding & preprocessing with scaling
4. Train/test split (90% training, 10% testing) for model preparation
5. Model training with Linear Regression, Lasso, Ridge, Random Forest, and XGBoost
6. Performance evaluation using MSE

## 🛠️ Tech Stack
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- XGBoost

## ✅ Outcome
Achieved accurate calorie prediction by comparing multiple regression models, with XGBoost and Random Forest delivering the best performance. Established a full ML pipeline from data preprocessing to model evaluation for regression problems.
