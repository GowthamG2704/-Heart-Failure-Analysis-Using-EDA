# Heart Failure Clinical Records Analysis

This project analyzes clinical data of heart failure patients to explore relationships between patient characteristics and mortality. The dataset contains 299 patient records with 13 attributes, including demographics, lifestyle factors, and medical test results. The analysis focuses on exploratory data analysis (EDA) using statistical techniques and visualizations to uncover patterns in the data.

## Project Overview

The goal of this project is to understand the factors contributing to heart failure outcomes (death or survival) using basic data analysis techniques. We do not use machine learning algorithms or advanced statistical models like survival analysis, focusing instead on EDA and visual insights.

## Dataset

The dataset used for this project consists of the following features:
- **age**: Age of the patient (years)
- **anaemia**: Whether the patient has anaemia (0 = No, 1 = Yes)
- **creatinine_phosphokinase**: Level of the CPK enzyme in the blood (mcg/L)
- **diabetes**: Whether the patient has diabetes (0 = No, 1 = Yes)
- **ejection_fraction**: Percentage of blood leaving the heart at each contraction
- **high_blood_pressure**: Whether the patient has high blood pressure (0 = No, 1 = Yes)
- **platelets**: Platelet count in the blood (kiloplatelets/mL)
- **serum_creatinine**: Level of serum creatinine in the blood (mg/dL)
- **serum_sodium**: Level of serum sodium in the blood (mEq/L)
- **sex**: Patient's gender (0 = Female, 1 = Male)
- **smoking**: Whether the patient smokes (0 = No, 1 = Yes)
- **time**: Duration of follow-up (days)
- **DEATH_EVENT**: Whether the patient died during the follow-up period (0 = No, 1 = Yes)

## Analysis Steps

1. **Data Loading & Cleaning**: Load the dataset, remove unnecessary columns, and handle missing values.
2. **Descriptive Statistics**: Summary statistics and distributions of key features like age, ejection fraction, and serum creatinine.
3. **Exploratory Data Analysis (EDA)**:
   - Pairplot to show relationships between features with respect to death event.
   - Bar plots for categorical variables like gender, smoking status, and death events.
   - Heatmap to identify correlations between numerical features.
4. **Visualization**:
   - Death event rate per gender.
   - Relationship between high blood pressure and age using categorical plots.
   - Smoking status and death events visualized using bar charts.

## Key Insights

- **Ejection Fraction**: Lower ejection fraction is strongly associated with increased mortality.
- **Serum Creatinine**: Elevated serum creatinine levels suggest higher risk of death, indicating a link to kidney function.
- **Age**: Older patients tend to have worse outcomes, but age alone is not a definitive predictor of death.
- **Smoking**: Smokers showed a higher death rate compared to non-smokers.
- **Gender**: Males experienced more deaths than females in this dataset.

## Visualizations

- **Pairplot**: Shows relationships between features with respect to the DEATH_EVENT variable.
- **Bar Plot**: Compares death events by gender and smoking status.
- **Catplot**: Shows the relationship between high blood pressure and age groups.

## Getting Started

### Prerequisites

Ensure you have the following Python libraries installed:

```bash
pip install pandas
pip install matplotlib
pip install seaborn
