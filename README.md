# DF_Regression-of-Used-Car-Prices
[DF 데이터 분석 프로젝트] predict the price of used cars based on various attributes


## Overview

### Objective
Predict used car prices based on various features using machine learning techniques.

### Dataset
- **Source**: (https://www.kaggle.com/competitions/playground-series-s4e9/overview)](https://www.kaggle.com/competitions/playground-series-s4e9/overview)
- **Training Data**: Includes features and corresponding car prices.
- **Test Data**: Unlabeled data for submission.

### Evaluation Metric
The competition uses **Root Mean Squared Error (RMSE)** to evaluate submissions.

---

## Repository Structure

- **`used_car_price_regression.ipynb`**: Jupyter Notebook containing the full workflow.
- **`README.md`**: Detailed guide to the repository.

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Analyzed data distributions, missing values, and outliers.
- Visualized relationships using histograms, scatter plots, and heatmaps.

### 2. Data Preprocessing
- **Missing Values**: Imputed missing data using mean and mode strategies.
- **Encoding**: Applied label and one-hot encoding for categorical features.
- **Outlier Handling**: Removed extreme outliers using statistical methods.
- **Scaling**: Standardized numerical features.

### 3. Feature Engineering
- Created new features based on domain knowledge.
- Performed feature selection using correlation analysis and importance scores.

### 4. Model Training
- Evaluated several models:
  - Linear Regression
  - Ridge and Lasso Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Used K-Fold cross-validation for robustness.
- Tuned hyperparameters with Grid and Randomized Search.

### 5. Model Selection
Selected the best-performing model based on RMSE scores for final predictions.

---

## Results

- **Best Model**: RMSE of the random forest model: 27.24
- **Test Predictions**: Submitted predictions for Kaggle evaluation.

---

## Usage Instructions

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `xgboost`

### Steps to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/used-car-price-regression.git
   ```
2. Navigate to the project folder:
   ```bash
   cd used-car-price-regression
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook used_car_price_regression.ipynb
   ```
4. Follow the steps in the notebook to reproduce the results.

---

