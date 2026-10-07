# Recipe Reviews and User Feedback

## Overview

This project focuses on analyzing recipe reviews and user feedback using Machine Learning. The goal is to understand user ratings and build classification models that can predict the rating given to a recipe.

## Objective

* Analyze recipe review data.
* Perform Exploratory Data Analysis (EDA).
* Handle missing values and outliers.
* Balance the target classes using SMOTE.
* Select important features.
* Train multiple Machine Learning classification models.
* Compare model performance using evaluation metrics.

## Dataset

**Dataset Name:** Recipe Reviews and User Feedback Dataset

* **Rows:** 18,182
* **Columns:** 15
* **Target Variable:** `stars`

The target variable represents the rating given by users.

### Target Distribution

| Rating  |  Count |
| ------- | -----: |
| 5 Stars | 13,829 |
| 0 Stars |  1,696 |
| 4 Stars |  1,655 |
| 3 Stars |    490 |
| 1 Star  |    280 |
| 2 Stars |    232 |

The dataset contains an imbalanced target distribution, with 5-star reviews being the majority class.

## Exploratory Data Analysis

The following analysis was performed:

* Dataset structure and shape
* Data types
* Missing value analysis
* Target variable distribution
* Numerical feature analysis
* Outlier detection

## Data Preprocessing

The following preprocessing techniques were applied:

* Missing value checking
* Outlier detection and treatment using the IQR method
* Target variable preparation
* Feature scaling
* Power transformation

## Handling Class Imbalance

Since the target classes were imbalanced, **SMOTE (Synthetic Minority Oversampling Technique)** was applied.

After SMOTE, all target classes were balanced with **13,829 samples per class**.

## Feature Selection

Feature selection was performed using **SelectKBest with ANOVA F-test**.

The selected features were:

* `RECIPE_NUMBER`
* `RECIPE_CODE`
* `CREATED_AT`
* `THUMBS_DOWN`
* `BEST_SCORE`

## Machine Learning Models

The following classification algorithms were implemented:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. AdaBoost Classifier
5. Gradient Boosting Classifier

## Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Classification Report

The models were compared to identify the most suitable classification approach for predicting recipe ratings.

> Note: Final numerical model performance values are not included here because they were not preserved in the submitted notebook output.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn
* Jupyter Notebook

## Project Structure

```text
Recipe-Reviews-and-User-Feedback/
│
├── Recipe Reviews and User Feedback Dataset.csv
├── Recipe_Reviews_and_User_Feedback.ipynb
├── README.md
└── project1_target_distribution.png
```

## How to Run

1. Clone this repository.
2. Open the Jupyter Notebook.
3. Make sure the dataset is placed in the correct directory.
4. Install the required Python libraries.
5. Run the notebook cells sequentially.

## Machine Learning Workflow

Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Outlier Treatment
   ↓
SMOTE
   ↓
Feature Selection
   ↓
Power Transformation
   ↓
Feature Scaling
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison

## Conclusion

This project demonstrates how Machine Learning can be applied to recipe reviews and user feedback data. Different classification algorithms were trained and evaluated to predict recipe ratings. Data preprocessing, class balancing, feature selection, and model evaluation were important steps in developing the classification workflow.
