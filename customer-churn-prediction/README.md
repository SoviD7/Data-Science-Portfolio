# Customer Churn Prediction

## Project Overview
Customer churn is a major challenge for subscription-based businesses. This project focuses on building a machine learning model to predict whether a customer is likely to churn based on demographic information, service usage, and billing details.

The goal is to identify key factors influencing churn and provide insights that can help businesses design effective customer retention strategies.

---

## Dataset
The dataset contains telecom customer information including service usage, billing details, and churn status.

**Dataset size**
- 7,043 customers
- 21 features

**Target Variable**
- `Churn`
  - 1 → Customer left the service
  - 0 → Customer stayed

---

## Project Workflow

### 1. Data Cleaning
- Removed identifier column (`customerID`)
- Converted `TotalCharges` to numeric
- Handled missing values

### 2. Data Preprocessing
- Encoded categorical variables using **One-Hot Encoding**
- Split dataset into **training (80%) and testing (20%) sets**

### 3. Model Training
Two models were trained and compared:

- Logistic Regression
- Random Forest Classifier

### 4. Model Evaluation
Models were evaluated using:
- Accuracy
- Confusion Matrix
- Precision, Recall, and F1-score

---

## Results

| Model | Accuracy |
|------|----------|
| Logistic Regression | ~78.5% |
| Random Forest | ~79% |

Both models performed similarly, with Random Forest providing slightly higher accuracy.

---

## Key Insights

Feature importance analysis revealed the most influential factors in predicting customer churn:

- **TotalCharges**
- **MonthlyCharges**
- **Tenure**
- **Contract type**
- **Internet service type**

Customers with **higher monthly charges and shorter tenure** are more likely to churn, while long-term customers tend to remain with the service.

---

## Business Impact
These insights can help telecom companies:

- Identify customers at high risk of churn
- Target retention campaigns more effectively
- Offer incentives or discounts to high-risk customers
- Improve long-term customer engagement strategies

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Repository Structure
