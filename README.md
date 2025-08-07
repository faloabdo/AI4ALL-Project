# AI4All Project - Diabetes Risk Prediction


This project analyzes key risk factors for diabetes and builds predictive models to assess individual diabetes risk based on health indicators from CDC's behavioral risk factor data.

## Background

This project was developed for AI4All's Applied AI program, where I applied machine learning techniques to public health data. My work focuses on:

- Identifying the most significant predictors of diabetes from 21 health indicators
- Comparing performance between different machine learning approaches
- Developing a practical risk assessment tool for potential clinical use

Using the Behavioral Risk Factor Surveillance System (BRFSS) 2015 dataset, we created models that can help with early diabetes risk detection and intervention planning.

## Key Findings

### 1. Top Risk Factors
Our analysis revealed these primary risk factors and their relative importance:

- **General Health (35% impact)**: Self-reported health status was the strongest predictor
- **High Blood Pressure (25%)**: Hypertension showed significant correlation
- **BMI (25%)**: Body Mass Index, especially values above 30
- **Age (15%)**: Particularly ages 45+ with non-linear risk increase

### 2. Model Performance Comparison
We evaluated two machine learning approaches:

| Model               | Accuracy | ROC AUC | Recall | Precision |
|---------------------|----------|---------|--------|-----------|
| Random Forest       | 75%      | 0.83    | 80%    | 73%       | 
| Logistic Regression | 75%      | 0.82    | 76%    | 74%       |

### 3. Risk Calculator Implementation
We developed an interactive web application with Real-time risk calculation and Personalized health recommendations using Streamlit.

## Next Steps

Future improvements planned:
- Compare with more recent BRFSS datasets (2020-2023)
- Test polynomial feature transformations
- Incorporate additional health indicators like family history
- Conduct clinical validation studies
- Expand to predict pre-diabetes risk

## Dataset

**Primary Dataset:**  
[CDC BRFSS 2015 Diabetes Dataset](https://www.kaggle.com/alexteboul/diabetes-health-indicators-dataset)  

**Exploratory Analysis:**  
[Dataset Notebook](https://www.kaggle.com/code/alexteboul/diabetes-health-indicators-dataset-notebook)

## Prepared by:

**Fuad Abdo** 

## Acknowledgments
