# MedicaInsure - Insurance Premium Prediction

## Problem Statement

**MedicaInsure** is a medical insurance provider. Leveraging customer information is of paramount importance for most businesses. In the case of an insurance company, analysis of customer attributes like age, sex, smoking habits, etc. can be crucial in making decisions regarding the premium amount to be charged.

The objective of this case study is to build a regression model that predicts insurance premium charges based on customer attributes.

## Dataset Description

The dataset contains information about insurance policyholders with the following attributes:

| Attribute | Description |
|-----------|-------------|
| `age` | Age of the policyholder |
| `sex` | Gender of the policyholder (male/female) |
| `bmi` | Body Mass Index of the policyholder |
| `children` | Number of children/dependents of the policyholder |
| `smoker` | Whether the policyholder is a smoker or not (yes/no) |
| `region` | Region where the policyholder belongs to (northeast, northwest, southeast, southwest) |
| `charges` | Premium charged to the policyholder (Target Variable) |

## Approach

1. **Data Loading & Exploration**: Load the dataset and understand its structure
2. **Exploratory Data Analysis (EDA)**: Visualize relationships between features and target variable
3. **Data Preprocessing**: Handle categorical variables, check for missing values
4. **Feature Engineering**: Create meaningful features if needed
5. **Model Building**: Build Linear Regression model
6. **Model Evaluation**: Evaluate using metrics like R², RMSE, MAE

## Key Insights

- Smoking status is expected to be a significant predictor of insurance charges
- Age and BMI are likely to have positive correlation with charges
- Regional differences may impact premium amounts

## Files

- `README.md` - This file with problem description
- `InsurancePremiumPrediction.ipynb` - Jupyter notebook with complete analysis
- `insurance.csv` - Dataset file (1340 records)

## Requirements

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```

## Usage

```bash
# Open Jupyter notebook
jupyter notebook InsurancePremiumPrediction.ipynb
```

## Technical Notes

- Use `random_state=1` for reproducibility in train-test splits and model training
- Import conventions:
  - `import pandas as pd`
  - `import numpy as np`
  - `import seaborn as sns`
  - `import matplotlib.pyplot as plt`
