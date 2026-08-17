Medical Insurance Cost Analysis

Overview

This project analyzes a medical insurance dataset to understand how demographic, lifestyle, BMI, and regional variables relate to medical insurance charges.

The notebook focuses on exploratory data analysis, data cleaning, feature engineering, preprocessing, and statistical feature analysis.

Objectives

Understand the distribution of insurance charges and demographic variables

Identify and remove duplicate records

Convert categorical variables into numerical representations

Engineer BMI-based categorical features

Standardize numerical variables

Measure relationships between features and insurance charges

Evaluate categorical features using Chi-square testing

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

SciPy

Scikit-learn

Dataset

The analysis works with 1,338 insurance records containing variables related to:

Age

Sex

BMI

Number of children

Smoking status

Region

Medical insurance charges

Analysis Performed

Exploratory Data Analysis

The notebook examines:

Dataset structure and data types

Descriptive statistics

Missing values

Numerical distributions

Category frequencies

Outliers using box plots

Correlations between numerical variables

Data Cleaning

Created a copy of the original dataset for preprocessing

Checked for missing values

Removed duplicate records

Converted categorical variables into numerical representations

Feature Engineering

BMI was transformed into four categories:

Underweight

Normal

Overweight

Obese

The BMI categories were then one-hot encoded for analysis.

Feature Preprocessing

Encoded sex as is_female

Encoded smoker as is_smoker

One-hot encoded regional categories

Standardized age, bmi, and children using StandardScaler

Statistical Analysis

Pearson correlation was calculated for selected numerical and encoded features against charges.

Categorical features were further evaluated using Chi-square tests after binning insurance charges into quartiles.

The analysis used an alpha level of 0.05 for statistical decision-making.

Key Analysis Areas

The project investigates relationships between insurance charges and:

Age

BMI

Number of children

Smoking status

Sex

Region

BMI category

Project Structure

medical-insurance-cost-analysis/
├── README.md
├── notebook/
│   └── Insurance_Projet.ipynb
├── data/
│   └── insurance.csv
└── requirements.txt

How to Run

Clone the repository.

Install the required Python packages.

Place insurance.csv in the expected data location.

Open Insurance_Projet.ipynb in Jupyter Notebook or JupyterLab.

Run the notebook cells sequentially.

Future Improvements

Build regression models to predict insurance charges

Compare Linear Regression, Random Forest, and Gradient Boosting models

Evaluate models using MAE, RMSE, and R²

Perform feature selection and hyperparameter tuning

Create an interactive dashboard for insurance-cost analysis

Author

Sagar Manohar
