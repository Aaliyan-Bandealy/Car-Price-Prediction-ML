# Car Price Prediction using Machine Learning

##  Project Overview

This project builds and compares multiple machine learning models to predict car prices using structured automotive data.

The workflow includes:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Selection using RFE
- Linear Regression
- K-Nearest Neighbors (KNN)
- Hyperparameter Tuning using GridSearchCV
- Model Evaluation and Comparison

---

##  Dataset

- Dataset: CarPrice.csv
- Records: 205 car models
- Features: Engine specifications, horsepower, fuel type, car body type, dimensions, and more
- Target Variable: `price`

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

##  Project Workflow

### 1️) Data Preprocessing
- Removed irrelevant columns (`car_ID`, `CarName`)
- Converted categorical variables using `pd.get_dummies`
- Split data into training and testing sets

### 2️) Exploratory Data Analysis
- Visualized price distribution
- Analyzed relationship between horsepower and price
- Compared price variations across car body types

### 3️) Model 1 – Linear Regression
- Trained baseline regression model
- Evaluated using:
  - Mean Squared Error (MSE)
  - R² Score

### 4️) Feature Selection – RFE
- Applied Recursive Feature Elimination
- Selected top 10 most important predictors
- Retrained Linear Regression using selected features

### 5️) Model 2 – KNN Regressor
- Trained KNN model on selected features
- Compared performance with Linear Regression

### 6️) Hyperparameter Tuning
- Used GridSearchCV to find optimal `n_neighbors`
- Evaluated tuned KNN model

---

##  Results

- Compared performance of:
  - Linear Regression
  - RFE + Linear Regression
  - KNN Regressor
  - Tuned KNN Model

- Identified the best-performing model based on lowest MSE and highest R².

---

##  How to Run the Project

1. Clone the repository:
   git clone https://github.com/yourusername/Car-Price-Prediction-ML.git

2. Navigate into the project folder:
   cd Car-Price-Prediction-ML

3. Install dependencies:
   pip install -r requirements.txt

4. Open the notebook:
   jupyter notebook notebooks/Car_Price_Prediction.ipynb
