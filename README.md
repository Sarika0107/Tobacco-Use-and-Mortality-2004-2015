# Tobacco Use and Mortality Prediction (2004–2015)

## Project Overview

Tobacco consumption remains one of the leading causes of preventable deaths worldwide. This project analyzes tobacco use patterns, smoking-attributable mortality, hospital admissions, economic indicators, prescription trends, and smoking prevalence data from 2004 to 2015.

The project combines data integration, exploratory data analysis (EDA), feature engineering, machine learning classification, and model interpretation techniques to predict whether smoking-attributable mortality levels are high or low and identify the factors contributing most significantly to tobacco-related deaths.

---

## Objectives

- Analyze tobacco-related mortality trends from 2004–2015.
- Examine the relationship between smoking prevalence and mortality.
- Study hospital admissions caused by smoking-related diseases.
- Investigate the impact of tobacco affordability and pricing.
- Evaluate the influence of smoking cessation prescriptions.
- Build machine learning models to predict high mortality risk.
- Identify key factors driving tobacco-attributable deaths.

---

## Dataset

The project integrates five datasets obtained from NHS Statistics on Smoking in England.

### Datasets Used

- Admissions Dataset
- Fatalities Dataset
- Smoking Prevalence Dataset
- Tobacco Metrics Dataset
- Prescription Dataset

### Key Features

- Year
- Sex
- Smoking Deaths
- Smoking Admissions
- Smoker Percentage
- Tobacco Price Index
- Retail Price Index
- Affordability of Tobacco Index
- Tobacco Expenditure Percentage
- Pharmacotherapy Prescriptions
- Pharmacotherapy Cost

### Target Variable

- High Mortality (Binary Classification)
  - 1 = High Smoking-Attributable Mortality
  - 0 = Low Smoking-Attributable Mortality

---

## Data Preprocessing

The following preprocessing steps were performed:

- Filtered smoking-attributable records.
- Standardized year formats across datasets.
- Aggregated mortality and admission statistics.
- Merged five datasets into a single analytical dataset.
- Handled missing values using forward-fill and backward-fill techniques.
- Converted numerical variables to appropriate formats.
- Removed incomplete observations.

---

## Feature Engineering

Several new features were created to improve model performance:

- High Mortality Target Variable
- Sex Encoding
- Year Trend Feature
- Admission-to-Death Ratio
- Smoking Percentage × Tobacco Affordability Interaction

These engineered features helped capture temporal patterns and relationships between smoking behavior and mortality outcomes.

---

## Exploratory Data Analysis (EDA)

### Key Insights

- Smoking-attributable deaths showed noticeable variation across years and genders.
- Male populations generally experienced higher smoking-related mortality than females.
- Smoking admissions were strongly associated with mortality rates.
- Tobacco affordability and smoking prevalence demonstrated meaningful relationships with mortality outcomes.
- Economic indicators and prescription trends influenced smoking behavior over time.

### Visualizations Performed

- Distribution of Smoking Deaths
- Smoking Deaths by Gender
- Feature Correlation Analysis
- Target Class Distribution
- Feature Importance Analysis
- SHAP Interpretation Visualizations

---

## Machine Learning Approach

### Models Implemented

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost Classifier
- LightGBM Classifier
- Support Vector Machine (SVM)

### Key Techniques

- Train-Test Split
- Stratified Cross Validation
- Standard Scaling
- Feature Engineering
- Binary Classification
- Model Comparison

---

## Model Evaluation

Models were evaluated using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

Cross-validation was used to ensure reliable and robust performance estimates.

---

## Best Performing Model

### Random Forest Classifier

The Random Forest model achieved the best overall performance by providing strong predictive accuracy while maintaining a balance between precision, recall, and ROC-AUC.

Detailed evaluation included:

- Confusion Matrix Analysis
- Feature Importance Ranking
- SHAP Explainability Analysis

---

## Feature Importance

The most influential predictors of high smoking-attributable mortality included:

- Smoking Admissions
- Smoker Percentage
- Tobacco Affordability Index
- Pharmacotherapy Prescriptions
- Net Ingredient Cost of Pharmacotherapies
- Admission-to-Death Ratio
- Tobacco Price Index
- Retail Price Index

These variables played a critical role in determining mortality risk.

---

## Explainable AI (XAI)

To improve model transparency, SHAP (Shapley Additive Explanations) was implemented.

### SHAP Analysis Included

- SHAP Summary Bar Plot
- SHAP Beeswarm Plot
- SHAP Waterfall Plot

These visualizations provided insights into how individual features influenced model predictions and mortality outcomes.

---

## Applications

This project can assist:

- Public Health Authorities
- Healthcare Policy Makers
- Tobacco Control Organizations
- Government Health Departments
- Medical Researchers

Potential applications include:

- Mortality Risk Assessment
- Tobacco Control Policy Planning
- Smoking Cessation Program Evaluation
- Healthcare Resource Allocation
- Public Health Monitoring

---

## Limitations

- Dataset covers only 2004–2015.
- Analysis is limited to available NHS tobacco-related statistics.
- External factors such as education, income, and lifestyle behaviors are not included.
- Results depend on historical data quality and reporting accuracy.
- Findings should be interpreted as analytical insights rather than causal conclusions.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- SHAP
- Jupyter Notebook

---

## Repository Contents

- Tobacco(s).ipynb → Complete analysis and machine learning workflow
- admissions.csv → Hospital admissions data
- fatalities.csv → Smoking-attributable deaths data
- metrics.csv → Tobacco economic indicators
- prescriptions.csv → Smoking cessation prescriptions
- smokers.csv → Smoking prevalence data
- README.md → Project documentation

---

## Author

**Sarika T A**  
Aspiring Data Analyst / Data Scientist

---

## Conclusion

This project successfully analyzed tobacco use and smoking-attributable mortality data between 2004 and 2015 by integrating multiple healthcare, economic, and behavioral datasets. Through comprehensive exploratory data analysis, important relationships were identified between smoking prevalence, hospital admissions, tobacco affordability, prescription treatments, and mortality outcomes.

Multiple machine learning algorithms were evaluated, including Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, XGBoost, LightGBM, and Support Vector Machines. Among these models, Random Forest demonstrated the strongest overall performance in predicting high mortality risk. Feature importance and SHAP analysis revealed that smoking admissions, smoking prevalence, tobacco affordability, and pharmacotherapy-related variables are among the most significant contributors to mortality outcomes.

Overall, the project demonstrates how machine learning and explainable AI can be applied to public health data to better understand tobacco-related risks and support evidence-based decision-making for tobacco control strategies.

---

## Future Improvements

- Incorporate additional demographic variables such as age, income, and education levels.
- Include regional and geographic health indicators for localized analysis.
- Extend the study using more recent tobacco and mortality datasets.
- Explore deep learning techniques for improved predictive performance.
- Build an interactive dashboard using Power BI or Tableau.
- Develop a real-time public health monitoring system.
- Integrate lifestyle and behavioral risk factors into the prediction framework.
- Perform longitudinal forecasting of smoking-related mortality trends.
- Enhance model explainability using advanced XAI techniques.
- Create policy simulation models to evaluate the impact of tobacco control interventions.

---
