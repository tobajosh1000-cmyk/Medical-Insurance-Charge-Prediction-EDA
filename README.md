# Medical-Insurance-Charge-Prediction-EDA

 ## Overview 
 An applied machine learning regression project that models medical insurance charges using demographic and lifestyle features(age, BMI, smoking, and status). The project implements a complete ML pipeline, including EDA, feature encoding, model training, evaluation, and interpretability to identify the strongest drivers of healthcare expenditure.

## Dataset
Source: Medical insurance dataset containing individual health records and corresponding insurance charges.

### Dataset Features
age: Age of primary beneficiary (integer)
sex: Gender (female/male)
bmi: Body mass index (float)
children: Number of dependents covered (integer)
smoker: Smoking status (yes/no)
region: Residential area in the US (northeast, southeast, southwest, northwest)
charges: Individual medical costs billed by insurance (float)
Dataset Size: 1,338 records × 7 columns

## Methodology

### 1 Exploratory Data Analysis (EDA)
Mean insurance charge: $13,270.42
High standard deviation ($12,110.01) indicates wide cost variability
BMI follows a typical distribution (mean: 30.66, std: 6.10)
Average number of children per policy: 1.09
BMI Categorization: Clinically meaningful BMI groups were created:
Age Grouping: Age was segmented into life stages:

### 2 Data Visualization
Distribution Analysis:
Insurance charges exhibit a strong right-skew
BMI follows a near-normal distribution with slight skew
Age distribution is relatively uniform
Most policyholders have 0–2 children

### Categorical Analysis:
Smokers incur significantly higher insurance charges
Gender shows moderate charge differences
Regional cost variations exist but are less pronounced
Relationship Analysis:
Strong positive relationship between age and charges
Clear separation between smoker and non-smoker cost distributions
BMI shows a non-linear relationship with charges

## Model Development
Linear Regression
Used as a baseline, interpretable regression model
Coefficient analysis enables direct feature impact interpretation
Smoking status exhibits the largest effect on predicted charges

### Model Evaluation
R² score for variance explanation
Residual analysis for model diagnostics
Cross-validation to assess robustness

## Results
### Key Findings:
Smoking Status – the strongest predictor of insurance charges
Age – consistent positive relationship with cost
BMI – moderate impact, especially at higher values
Region – Southeast shows the highest average charges
Children – moderate influence on overall cost

### Model Interpretation:
Smokers pay approximately 3–4× more than non-smokers
Each additional year of age increases charges by ~$250–300
BMI above 30 significantly increases medical expenses
Regional differences account for ~$1,000–2,000 variation



