# Heart Disease Analysis

<div align="center">

<img src="heart.png" alt="drawing" width="300"/>

</div>

## Overview
Comprehensive analysis of 1,025 patient records to identify key factors contributing to heart disease. Built machine learning models achieving strong predictive accuracy to support early diagnosis and medical decision-making in cardiovascular care.

## Dataset Overview
- **Size**: 1,025 patient records with 14 clinical attributes covering demographics, test results, and disease presence.
- **Target Variable**: Binary classification where 1 indicates presence of heart disease (51.3% of patients) and 0 indicates absence (48.7%).
- **Key Features**: Age (29-77 years, avg 54), sex (69.6% male), chest pain type (cp), resting blood pressure (trestbps), cholesterol (chol), fasting blood sugar (fbs), resting ECG results (restecg), max heart rate (thalach), exercise-induced angina (exang), ST depression (oldpeak), slope, number of major vessels (ca), and thalassemia (thal).
- **Data Quality**: Complete dataset with no missing values, all numeric features ready for modeling.
- **Clinical Ranges**: Blood pressure ranges from 94-200 mmHg, cholesterol from 126-564 mg/dl, and max heart rate from 71-202 bpm.
- **Target Distribution**: Fairly balanced dataset with 526 heart disease patients and 499 healthy individuals.

## Analysis
- **Exploratory Data Analysis (EDA)**:  
  - Examined distributions of all clinical features, finding older patients (avg 56.6 years) with higher risk of heart disease compared to younger healthy patients (avg 52.6 years).
  - Identified that heart disease patients have lower max heart rates (avg 139 bpm) versus healthy patients (avg 158 bpm), indicating reduced cardiac capacity.
  - Discovered males comprise 82.6% of diseased patients, showing significant gender disparity in heart disease prevalence.

- **Visualizations**:  
  - Created correlation heatmaps showing strong relationships between chest pain type, exercise angina, and disease presence.
  - Built distribution plots, boxplots, and count plots to visualize differences between diseased and healthy groups across all clinical parameters.
  - Analyzed chest pain patterns, with type 0 (typical angina) most common in diseased patients while type 2 appears more in healthy individuals.

- **Feature Analysis**:  
  - ST depression (oldpeak) significantly higher in diseased patients (avg 1.59) vs healthy (avg 0.59), indicating cardiac stress.
  - Major vessels colored by fluoroscopy (ca) show diseased patients average 1.17 blocked vessels compared to 0.34 in healthy patients.
  - Examined combinations of chest pain type, fasting blood sugar, and exercise angina to identify high-risk patient profiles.

- **Machine Learning Models**:  
  - Trained multiple classification algorithms including Logistic Regression, Random Forest, and potentially SVM or KNN for heart disease prediction.
  - Performed feature importance analysis to identify top predictors like chest pain type, major vessels, thalassemia, and oldpeak values.
  - Split data into training and test sets, evaluated model performance using accuracy, precision, recall, and F1-scores to ensure reliable predictions for clinical use.

## How to Use
- Clone the repository:
  ```git
    git clone https://github.com/PratyushPuri/Heart-Disease-Analysis.git
  ```
- Install required dependencies:
  ```python
  pip install -r requirements.txt
  ```
- Common libraries include pandas, numpy, seaborn, matplotlib, and scikit-learn.
- Open `heart-disease-analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
- Run cells sequentially from top to bottom for data loading, cleaning, visualization, and model training.
- Original Kaggle notebook:  
[heart-disease-analysis](https://www.kaggle.com/code/pratyushpuri/heart-disease-analysis)
- Customize the analysis:  
- Experiment with different ML algorithms or ensemble methods to improve prediction accuracy.
- Add new features like BMI or lifestyle factors if available.
- Tune hyperparameters using GridSearchCV or RandomizedSearchCV for optimal model performance.
- Deploy models using joblib or pickle for integration into healthcare systems or diagnostic tools.

## Author & Contact
- Name: `Pratyush Puri`  
- Contact: `pratyushpuri17@gmail.com`  
- LinkedIn: [https://www.linkedin.com/in/pratyushpuri](https://www.linkedin.com/in/pratyushpuri)




  
