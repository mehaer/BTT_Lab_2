# Airbnb NYC Listings: Data Preparation & Exploration

This project focuses on the **data understanding** and **data preparation** phases of the machine learning life cycle.  
Using the Airbnb NYC “listings” dataset, I prepared data for an upcoming **regression problem** — cleaning, transforming, and exploring relationships between features and price.

---

## Project Overview

Before building any machine learning model, the data must be thoroughly understood and prepared.  
This lab demonstrates essential preprocessing techniques such as **handling outliers**, **imputing missing data**, and **encoding categorical variables**.

The goal was to create a cleaned, structured dataset ready for future modeling while exploring how various features relate to the target variable: **listing price**.

---

## Tasks Completed

### 1. Build the Data Matrix & Define the ML Problem
- Loaded the **Airbnb NYC listings dataset** into a DataFrame.  
- Defined the **label** (`price`) and converted it to a numeric type suitable for regression.  
- Identified and selected relevant **features** for analysis.

### 2. Clean the Data
- **Handled outliers** using **winsorization** to reduce the impact of extreme values on the target variable.  
- **Imputed missing values** with the **mean** for each column to ensure dataset completeness.  
- **Applied one-hot encoding** to convert categorical features into numerical format for modeling compatibility.

### 3. Explore the Data
- Computed correlations between features and the label to identify the **two most correlated features**.  
- Built **bivariate scatter plots** to visualize relationships between features and price.  
- Observed slight upward trends between:
  - **Number of accommodations** and **price**  
  - **Number of bedrooms** and **price**

### 4. Analysis & Insights
- The scatterplots revealed **weak positive correlations** between the top two features and price — meaning as accommodations or bedrooms increase, the price tends to rise slightly.  
- Despite weak correlations, both features are **logically important** and should be included in future regression models.

---

## Additional Observations

- Features like **description** and **neighborhood overview** contain **unstructured text** that could be useful with **NLP preprocessing** (e.g., sentiment or keyword extraction).  
- Features such as **host name** may not provide meaningful predictive value and can be excluded.  
- Further steps before modeling could include:
  - Scaling numerical features  
  - Encoding or processing additional categorical variables  
  - Engineering new features (e.g., price per bedroom or review score categories)

---

## Tools & Libraries Used

- **Python 3.x**
- **Pandas** – Data manipulation  
- **NumPy** – Numerical computation  
- **Matplotlib / Seaborn** – Visualization  
- **scikit-learn** – One-hot encoding and preprocessing utilities  
- **SciPy** – Winsorization for outlier handling

---

## Key Takeaways

- Data cleaning and transformation are critical to reliable model training.  
- Outlier handling and missing value imputation improve data quality and stability.  
- Even weak correlations can provide valuable insights when supported by logical reasoning.  
- Textual features may enhance future models with proper feature engineering.


