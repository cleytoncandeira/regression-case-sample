# Regression Analysis Case (Junior Data Scientist)

This repository contains my solution for **Problem 3: Regression Analysis**, which was part of a selective process for a Junior Data Scientist position. My solution for this challenge helped me advance to the interview stage.

---

## Context and Goal

A supermarket company wants to verify if it is adhering to a new internal policy aimed at preventing significant salary discrimination according to the location of its employees. The dataset provided (`1stPhase-SelectiveProcess-Data Science-Data Base.csv`) includes information such as salaries, location (urban center vs. rural/“interior”), and other relevant features.

**Key Objective**  
Determine whether employees in different locations (**CENTRO** vs. **INTERIOR**) have significantly different salaries and assess the primary variables that influence salary composition.

---

## Approach Overview

1. **Exploratory Data Analysis (EDA)**  
   - **Data Inspection:** Examine the distribution of numeric and categorical variables using descriptive statistics (mean, median, standard deviation) and data visualization (box plots, histograms, scatter plots).  
   - **Initial Checks:** Test normality for numeric variables (Shapiro-Wilk, Kolmogorov-Smirnov, Anderson-Darling) and apply suitable tests (e.g., chi-square) for categorical variables.  
   - **Categorical Variables:** Specifically analyze **LOCAL** (nominal: CENTRO vs. INTERIOR) and its relationship to **SALARIO_MENSAL**.

2. **Feature Engineering**  
   - **Dimensionality Reduction & Bias Minimization:** Convert numeric variables to categorical groups when appropriate (e.g., **IDADE** → age brackets) to mitigate linear correlation with **TEMPOCASA**.  
   - **Transformations:** Apply log, Box-Cox, or root transformations to normalize skewed distributions.

3. **Data Encoding & Scaling**  
   - Standardize/scale variables to a uniform metric.  
   - Encode ordinal vs. nominal variables correctly for modeling.

4. **Correlation Analysis**  
   - Use **Spearman**, **Pearson**, and **Kendall** correlation methods to detect and address multicollinearity, determining which regressors are most significant for **SALARIO_MENSAL**.

5. **Modeling & Validation**  
   - **Initial Model:** Ordinary Least Squares (OLS) from classical econometrics.  
   - **Alternative Approaches:** Machine Learning regressions (Decision Tree, SVM, ElasticNet), and if needed, Deep Learning (Sequential Neural Networks) for complex data structures.  
   - **Key Evidence:** Determine the significance of **LOCAL** in predicting **SALARIO_MENSAL** and identify other influential factors in salary composition.



