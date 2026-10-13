# 🎓 College Admission Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting college admission outcomes using Machine Learning and data analysis techniques. It covers the complete data science workflow, including data cleaning, Exploratory Data Analysis (EDA), feature engineering, model training, and performance evaluation.

The project compares a baseline Logistic Regression model with an improved HistGradientBoosting classifier to evaluate changes in predictive performance.

## 🎯 Project Objectives

- Clean and preprocess college admission data.
- Analyze applicant characteristics and admission trends.
- Explore relationships between academic performance and admission outcomes.
- Visualize data distributions, correlations, and outliers.
- Engineer new features to improve model performance.
- Train and compare baseline and improved classification models.
- Evaluate performance using multiple classification metrics.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Environment:** Google Colab / Jupyter Notebook
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## 📊 Dataset Features

The notebook analyzes the following applicant-related features:

- Age
- Gender
- Category
- State
- Preferred Stream
- Entrance Exam
- Entrance Score
- Board Percentage
- Extracurricular Score
- Scholarship Eligibility
- Admission Probability

**Target Variable:** `admission_status`

The target identifies applicants as `admitted` or `rejected`.

## 🧹 Data Cleaning and Preprocessing

The project includes:

- Dataset inspection and descriptive statistics
- Missing-value analysis and treatment
- Duplicate-row removal
- Standardization of column names and categorical text
- Removal of the student identifier from predictive features
- Outlier detection using the Interquartile Range (IQR) method
- Numerical feature scaling and categorical encoding

The cleaned dataset is exported as `College_Admission_cleaned.csv`.

## 📈 Exploratory Data Analysis (EDA)

The notebook contains 27 visualizations and analytical outputs, including:

- Admission status distribution
- Age, entrance score, and board percentage distributions
- Applicant distribution by gender, category, and state
- Preferred stream and entrance exam analysis
- Scholarship eligibility distribution
- Admission status comparisons across applicant groups
- Admission probability and academic score boxplots
- Entrance score versus board percentage scatter plot
- Correlation heatmap
- Numerical feature boxplots
- Pairplot for selected numerical features
- Admission-rate analysis for categorical features
- Baseline versus improved model comparison
- Confusion matrix and ROC curve

These analyses help identify patterns and relationships in the dataset.

## 🤖 Machine Learning Models

### 1. Baseline Model — Logistic Regression

The baseline model uses a preprocessing pipeline with numerical imputation, standardization, categorical imputation, and one-hot encoding.

### 2. Improved Model — HistGradientBoosting Classifier

The improved model uses feature engineering and a HistGradientBoosting classifier to capture more complex relationships in the data.

### Feature Engineering

The project creates additional features, including:

- Academic Average
- Score–Board Gap
- Entrance–Board Product
- Extracurricular Ratio
- Age Squared

## 📏 Model Evaluation Metrics

Both models are evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted admissions that are correct.
- **Recall:** Proportion of actual admitted applicants correctly identified.
- **F1 Score:** Harmonic mean of precision and recall.
- **ROC-AUC:** Ability to distinguish between admission outcomes.

The notebook also generates confusion matrices, classification reports, ROC curves, and a comparison chart.

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Upload the dataset

The notebook uses Google Colab's file upload interface. Prepare your dataset as a CSV file containing the expected columns, including `admission_status`.

When running locally, replace the Google Colab upload code with:

```python
import pandas as pd

df = pd.read_csv("your_dataset.csv")
```

### 4. Run the notebook

Open `Major_Project_3_Complete_Cleaning_EDA.ipynb` in Google Colab or Jupyter Notebook and execute the cells in order.

## 📁 Repository Structure

```text
College-Admission-Prediction/
│
├── Major_Project_3_Complete_Cleaning_EDA.ipynb
├── College_Admission_cleaned.csv
└── README.md
```

The cleaned CSV is generated when the notebook runs successfully.

## 🚀 Future Improvements

- Hyperparameter tuning and cross-validation
- More robust feature selection
- Explainability using feature importance or SHAP
- A web interface for admission predictions
- Testing on independent datasets
- Fairness and bias evaluation across applicant groups

## ⚠️ Important Note

This is an educational Machine Learning project. Admission predictions are estimates, not guarantees. The model should not be used as the sole basis for real admission decisions, and its fairness and reliability should be evaluated before practical use.

## 👨‍💻 Author

**Ariyan Khan**

B.Tech — Computer Science Engineering

Interested in Data Science, Machine Learning, and Artificial Intelligence.
