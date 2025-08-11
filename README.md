# Project: Personality Prediction (Extrovert vs Introvert)
**Dataset:** [Kaggle – Extrovert vs Introvert Behavior Data](https://www.kaggle.com/datasets/rakeshkapilavai/extrovert-vs-introvert-behavior-data)

This project builds a machine learning pipeline to predict whether a person is **Extrovert** or **Introvert** based on behavioral survey data.

## Workflow
### 1. Data Understanding
* Explore columns, check data types, describe numerical & categorical features, detect errors.

### 2. Data Cleaning
* Dealing with any errors found

### 3. Feature Extraction
* Extract Feature based on domain knowledge

### 4. Analysis
* Perform **Univariate Analysis**.
* Perform **Bivariate Analysis**.

### 5. Data Preprocessing
* Handle duplicates, missing values, and outliers.
* Encode features:
  * Ordinal → `OrdinalEncoder`, `LabelEncoder`
  * Nominal (<7 uniques) → One-Hot Encoding
  * Nominal (>7 uniques) → Binary Encoding
*  Dealing with Balance dataset.
* Scale features with `StandardScaler`, `MinMaxScaler`, `RobustScaler`.

### 6. Modeling
* Tested multiple models: Logistic Regression, KNN, GaussianNB, SVC, Decision Tree, Bagging, Gradient Boosting, Voting Classifier.
* Selected **StackingClassifier** combining:
  * XGBoost
  * CatBoost
  * Gradient Boosting
  * Voting Classifier combining:
    * SVC
    * GaussianNB
    * Logistic Regression

### 7. Results
* Validation Accuracy: **93.03%**
* Test Accuracy: **91.45%**
* Precision, Recall, F1-Score above 87%.
* PR curve evaluated to find the best decision threshold.
* Final model saved for deployment.
  
 
