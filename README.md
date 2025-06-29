# Accident Severity Risk Prediction

This project focuses on predicting the severity of road traffic accidents by analyzing the interaction between driver age and environmental risk factors such as weather, lighting, and road surface conditions. The study was conducted as part of a research initiative under the Department of Computer Science and Engineering, Amrita Vishwa Vidyapeetham, Coimbatore.

## Objective

To investigate how age-related driving behaviors interact with environmental conditions and develop a machine learning model to predict the severity of accidents. The findings aim to assist policymakers in creating age-specific safety interventions and improve road infrastructure planning.

## Dataset

The dataset used is a licensed traffic accident dataset containing features such as:

- Driver age
- Weather conditions
- Lighting conditions
- Road surface conditions
- Accident severity (target variable)

Data preprocessing steps included:
- Removal of duplicates
- Encoding categorical variables
- Normalization and scaling

## Methodology

1. **Data Preprocessing**
   - Handled missing values, performed normalization, and encoded categorical features.

2. **Model Development**
   - Trained and evaluated three models: Decision Tree, Random Forest, and Logistic Regression.
   - The Decision Tree model achieved the highest accuracy (85%) and was selected for further analysis.

3. **Model Interpretation**
   - Applied SHAP (SHapley Additive exPlanations) to interpret model predictions and understand feature importance.

4. **Subgroup Analysis**
   - Divided the dataset into four age groups: Under 18, 18–30, 31–50, and 51+.
   - Built separate models for each group to analyze age-specific vulnerabilities.

5. **Association Rule Mining**
   - Extracted frequent patterns and rules to identify high-risk condition combinations.

## Key Findings

- Young drivers (18–30) are more prone to serious accidents in poor lighting and wet conditions.
- Older drivers (51+) face higher risk in adverse weather and low-visibility residential areas.
- Middle-aged drivers (31–50) experience severe crashes mostly due to environmental factors rather than behavioral ones.
- Night-time and wet road combinations significantly increase accident severity across all age groups.

## Technologies Used

- Python
- scikit-learn
- pandas, NumPy
- SHAP
- mlxtend (for association rule mining)
- Matplotlib, Seaborn (for visualization)

## Results

- Decision Tree model accuracy: **85%**
- Effective in segmenting and analyzing age-specific crash patterns.
- Supports targeted road safety policy formulation.
