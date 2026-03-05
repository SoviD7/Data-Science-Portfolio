# House Price Prediction

## Project Overview
This project focuses on predicting house prices using machine learning techniques. The objective is to analyze property characteristics such as living area, number of bedrooms, bathrooms, and house condition to estimate housing prices.

The project demonstrates a complete machine learning workflow including data exploration, preprocessing, model training, evaluation, and interpretation of results.

---

## Dataset
The dataset contains information about residential properties including structural details, property condition, and location attributes.

**Dataset size**
- 4,600 records
- 18 features

**Target Variable**
- `price` – the selling price of the house

**Important Features**
- bedrooms
- bathrooms
- sqft_living
- sqft_lot
- floors
- waterfront
- view
- condition
- yr_built
- yr_renovated
- city
- statezip

---

## Project Workflow

### 1. Data Exploration
Initial exploration was performed to understand the structure of the dataset, feature distributions, and relationships between variables.

### 2. Data Cleaning
- Removed unnecessary columns such as `street` and `country`
- Encoded categorical variables (`city`, `statezip`) using one-hot encoding
- Checked for missing values and verified dataset consistency

### 3. Feature Engineering
Prepared the dataset for modeling by separating features (`X`) and target variable (`y`) and splitting the data into training and testing sets.

### 4. Model Training
Two regression models were trained:

- Linear Regression
- Random Forest Regressor

### 5. Model Evaluation
Model performance was evaluated using standard regression metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### 6. Feature Importance
Feature importance analysis from the Random Forest model helped identify the most influential factors affecting house prices.

---

## Key Insights
Feature importance analysis revealed that the most significant predictors of house prices include:

- **sqft_living**
- **sqft_above**
- **bathrooms**
- **bedrooms**

These results indicate that property size and interior space are major drivers of housing value.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Repository Structure
