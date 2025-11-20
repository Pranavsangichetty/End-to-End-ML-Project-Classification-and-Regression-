🚀 End-to-End Machine Learning Project — Classification & Regression

A complete end-to-end Machine Learning project performing both Classification and Regression on the given dataset using Scikit-Learn pipelines.
This project showcases preprocessing, feature engineering, model training, comparisons, evaluations, and business insights.

📌 Project Overview

This project explores two types of Machine Learning tasks using the same dataset:

🔹 1. Classification Task

Predict whether an event belongs to class 1 or 0.

🔹 2. Regression Task

Predict a continuous output and compare performance across multiple regression algorithms.

The project is fully implemented in Jupyter Notebook (ML_Project(Cls&Reg).ipynb), including data cleaning, preprocessing, model training, evaluation, and visualization.

🎯 Objectives

✔ Build both Regression and Classification pipelines

✔ Apply data preprocessing using ColumnTransformer

✔ Train multiple ML models and compare performance

✔ Visualize model performance using horizontal bar comparison charts

✔ Provide insights from both regression and classification outputs

✔ Save final predictions and model comparison graphs

🧼 1. Data Cleaning & Preparation

The following cleaning steps were performed:

Removed duplicates

Handled missing values using:

Median imputation (numerical)

Constant/OHE imputation (categorical)

Dropped identifier columns

Standardized numerical features

Encoded categorical variables:

Low-cardinality → One-Hot Encoding

High-cardinality → Ordinal Encoding

Split data into training/testing sets

Built pipelines for both regression and classification tasks

🧠 2. Machine Learning Models Used
🔹 Regression Models

Linear Regression	✔

Ridge Regression	✔

Lasso Regression	✔

Decision Tree Regressor	✔

Random Forest Regressor	✔

KNN Regressor	✔

AdaBoost Regressor	✔

XGBRegressor	✔

CatBoost Regressor	✔

🔹 Classification Models

Logistic Regression	✔

Random Forest Classifier	✔

XGBoost Classifier	✔

CatBoost Classifier	✔

AdaBoost Classifier	✔

⚙️ 3. End-to-End Preprocessing Workflow

All transformations are combined using Scikit-Learn’s Pipeline + ColumnTransformer:

✨ Numerical Features

Median Imputation

Standard Scaling

✨ Categorical Features

One-Hot Encoding (low cardinality)

Ordinal Encoding (high cardinality)

This ensures cleaner, faster, and repeatable model training.

📊 4. Model Evaluation

🔹 Regression (R² Score Comparison)

A clean green–orange horizontal bar chart (model_comparison.png) was generated, similar to:

Linear Regression: 87.5%

Ridge: 87.5%

CatBoost: 85.6%

Random Forest: 83.8%

XGBRegressor: 81.8%

AdaBoost: 81.8%

Lasso: 81.6%

KNN: 76.5%

Decision Tree: 67.6% (highlighted in orange as worst)

This plot is included in the project as:

model_comparison.png

🔹 Classification Metrics
Metric	Score
|Accuracy	|~0.85 – 0.93 (depending on model)|
|Precision	|~0.81 – 0.92|
|Recall	|~0.78 – 0.89|
|F1-Score	|~0.80 – 0.90|
|ROC-AUC	|~0.92 – 0.97|

The classification task provides strong predictive performance and reliable business insights.

🔍 5. Project Insights

🔹 Regression

Tree-based models (Random Forest, XGB, CatBoost) outperform linear models.

Decision Tree alone underperforms due to high variance.

🔹 Classification

Ensemble models (Random Forest, AdaBoost, XGB, CatBoost) deliver the best balance of accuracy and recall.

Logistic Regression provides clean interpretability, ideal for business decisions.

📁 6. Outputs Generated

The notebook generates the following files:

model_comparison.png

metrics_df.csv

predictions_regression.csv

predictions_classification.csv


These files contain the final predictions and model comparisons.

🧩 7. Technologies Used

Python

NumPy, Pandas

Matplotlib

Scikit-Learn

XGBoost

CatBoost

Jupyter Notebook

