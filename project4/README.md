# Titanic Survival Prediction

## Objective
Build and optimize a machine learning model to predict whether a passenger survived the sinking of the Titanic based on their attributes. The project also compares the performance of a **Random Forest Classifier** and a **Logistic Regression** model.

## Dataset
The projecct uses the Titanic Survival Dataset from the Seaborn library. The target variable is `survived`, where 1 means the passenger survived, and 0 means they did not.

## Key Steps
1. **Select Features**: (from the dataset)
   - Relevant features: `pclass`, `sex`, `age`, `sibsp`, `parch`, `fare`, `class`, `who`, `adult_male`, `alone`
   - Target variable: survived
2. **Split Data**:
   The data is split into training and testing sets, with stratification to handle the slight class imbalance in the target variable.
3. **Define Preprocessing**:
   Separate pipelines for numerical and categorical features are created. A `ColumnTransformer` is used to combine these transformers into a single preprocessor.
4. **Create Model Pipeline**:
   A `Pipeline` is created to combine the preprocessor with a machine learning classifier, initially a `RandomForestClassifier`.
5. **Train and Optimize**:
   `GridSearchCV` is used with a stratified k-fold cross-validation (`cv=5`) to train the pipeline and find the optimal hyperparameters for the classifier.
6. **Evaluate Performance**:
   The model's performance is evaluated using a classification report and a confusion matrix on the unseen test data.
7. **Compare Models**:
   The classifier in the pipeline is replaced with a `LogisticRegression` model, and its performance is evaluated and compared to the Random Forest model.

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib

## Outcome
The project successfully builds and optimized two classification models. The results show a slight performance edge for the **Logistic Regression** model. The project highlights the importance of using a comprehensive pipeline and understanding how different models arrive at their predictions.
