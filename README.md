# Diabetes Risk Prediction Tool
### AI4All Project | Team Fuad Abdo

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B.svg?logo=Streamlit&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)

## Project Overview
A machine learning system that identifies key diabetes risk factors and provides personalized risk assessments through an interactive web application.

## Key Features
- **Predictive Modeling**: 
  - Random Forest (AUC: 0.83)
  - Logistic Regression (AUC: 0.82)
- **Risk Calculator**:
  - Interactive Streamlit interface
  - Personalized risk scores (5%-95% range)
  - Clinical recommendations
- **Feature Analysis**:
  - Identified 4 dominant risk factors
  - Fairness validation across demographics

## Technical Implementation
```python
def predict_risk(bmi, age, health, bp):
    # Non-linear age mapping
    age_risk = {1:0.1, 2:0.15, ..., 13:0.9}[age]
    
    # Weighted factors
    risk_score = (bmi*0.25 + age_risk*0.15 + 
                 health*0.35 + bp*0.25)
    
    return 1/(1 + exp(-4*(risk_score - 0.5)))
