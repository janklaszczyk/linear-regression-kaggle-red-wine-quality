# Red Wine Quality - Explanatory Model

## Overview
This project focuses on building an explanatory model using a multilinear regression approach to identify the physicochemical variables that statistically significantly influence the quality of red wine. The model analyzes relationships between the independent variables (features) and the dependent variable (quality score), helping uncover which physicochemical properties are most impactful on wine quality.

---

## Context
The dataset is based on the red variant of the Portuguese "Vinho Verde" wine. It includes physicochemical properties (inputs) and sensory data (outputs). Detailed information about grape types, wine brand, or selling prices is not included due to privacy and logistic issues.

This dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality) also available on kaggle (https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009) and was described in the paper:

> **Reference**:  
P. Cortez, A. Cerdeira, F. Almeida, T. Matos, and J. Reis. *Modeling wine preferences by data mining from physicochemical properties.* Decision Support Systems, Elsevier, 47(4):547-553, 2009.

---

## Dataset Content
The dataset contains **no missing values** and includes the following variables:

### **Independent Variables** (Physicochemical tests):
1. **Fixed Acidity**  
2. **Volatile Acidity**  
3. **Citric Acid**  
4. **Residual Sugar**  
5. **Chlorides**  
6. **Free Sulfur Dioxide**  
7. **Total Sulfur Dioxide**  
8. **Density**  
9. **pH**  
10. **Sulphates**  
11. **Alcohol**

### **Dependent Variable** (Sensory data):
12. **Quality**: A score between 0 and 10 based on wine taste evaluations.

---

## Project Objectives
1. **Perform Data Exploration**:  
   - Analyze relationships between features using visualizations (e.g., correlation heatmaps).  
   - Investigate potential multicollinearity among independent variables.

2. **Model Building**:  
   - Fit a multilinear regression model using `statsmodels`.  
   - Identify statistically significant variables influencing wine quality.

3. **Performance Evaluation**:  
   - Split data into training and testing sets to assess generalizability.  
   - Use evaluation metrics such as R-squared, Mean Squared Error, and residual analysis.

4. **Insights and Recommendations**:  
   - Highlight which physicochemical properties impact wine quality the most focusing on **Alcohol concentration**
   - Provide actionable insights for winemakers based on model findings.

---

## Tools and Libraries
- **Python Libraries**:  
  - `pandas`, `numpy` for data manipulation  
  - `matplotlib`, `seaborn` for visualizations  
  - `statsmodels` for regression modeling and statistical analysis

---

## How to Run
1. Clone this repository and ensure the dataset file (`winequality-red.csv`) is in the same directory.  
2. Install required libraries using `pip install -r requirements.txt`. 

---

## Results and Key Insights
- Key statistically significant variables influencing wine quality will be displayed, along with their coefficients and p-values.
- The residual plots and other diagnostic tools will assess the model's goodness of fit and assumptions.

---