# A/B Testing for Website Conversion

## Project Overview
This project analyzes the results of an A/B experiment conducted to determine whether a new website landing page leads to higher user conversion compared to the existing page.

The goal is to use statistical hypothesis testing to evaluate whether the observed difference in conversion rates is statistically significant.

---

## Dataset
The dataset contains information about users who were randomly assigned to either the control group (old landing page) or the treatment group (new landing page).

**Dataset size**
- ~294,000 user records
- 5 columns

**Important Columns**
- `user_id` – unique identifier for each user
- `group` – control or treatment group
- `landing_page` – old_page or new_page
- `converted` – whether the user converted (1) or not (0)
- `timestamp` – time of user visit

---

## Project Workflow

### 1. Data Exploration
Initial analysis was performed to understand dataset size, group distribution, and conversion rates.

### 2. Data Cleaning
- Removed mismatched rows where group assignment did not match the landing page
- Verified data consistency
- Calculated conversion rates for control and treatment groups

### 3. Hypothesis Testing

**Null Hypothesis (H₀):**  
The new landing page does not improve conversion rate.

**Alternative Hypothesis (H₁):**  
The new landing page improves conversion rate.

A **two-proportion Z-test** was applied to compare conversion rates between the two groups.

### 4. Statistical Testing
The Z-test was used to calculate:

- Z-statistic
- p-value

The significance level (α) was set to **0.05**.

---

## Results

| Group | Conversion Rate |
|------|------|
| Control | ~12.04% |
| Treatment | ~11.89% |

**p-value ≈ 0.19**

Since the p-value is greater than the significance level (0.05), we fail to reject the null hypothesis.

---

## Conclusion
The analysis shows that the new landing page does **not produce a statistically significant improvement** in conversion rate. Therefore, based on this experiment, there is insufficient evidence to support replacing the existing landing page with the new design.

This project demonstrates how statistical hypothesis testing can be applied to evaluate business experiments and support data-driven decision making.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Statsmodels
- Matplotlib
- Jupyter Notebook

---

## Repository Structure
