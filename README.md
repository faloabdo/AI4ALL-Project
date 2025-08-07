# AI4All Project - Diabetes Risk Prediction

This project analyzes key risk factors for diabetes and builds predictive models to assess individual diabetes risk based on health indicators.

## Background
This project was developed for AI4All, and it applies machine learning to CDC health data to:
- Identify the strongest predictors of diabetes
- Compare model performance (Random Forest vs Logistic Regression)
- Build a clinical risk assessment tool

Using the BRFSS 2015 dataset (253,680 respondents), we focus on predicting diabetes risk to help with early intervention.

## Key Findings
1. **Top Risk Factors**:
   - General Health (35% impact)
   - High Blood Pressure (25%)
   - BMI (25%)
   - Age (15%)

2. **Model Performance**:
   | Model               | Accuracy | ROC AUC |
   |---------------------|----------|---------|
   | Random Forest       | 75%      | 0.83    |
   | Logistic Regression | 75%      | 0.82    |

3. **Risk Calculator**:
   - Streamlit web app
 
## Next Steps
- Incorporate more health indicators
- Test with polynomial features
- Develop mobile version
- Clinical validation study

## Dataset
Origianl dataset: [CDC BRFSS 2015](https://www.kaggle.com/alexteboul/diabetes-health-indicators-dataset)  
Dataset notebook: (https://www.kaggle.com/code/alexteboul/diabetes-health-indicators-dataset-notebook)  


Fuad Abdo
