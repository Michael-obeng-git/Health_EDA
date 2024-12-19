# Exploratory Data Analysis on a heart disease dataset

## Objective

This project is an Exploratory Data Analysis (EDA) on heart disease dataset, the dataset is located in the data folder.
The data contains information on heart health indicators, including demographic, clinical, 
and lifestyle variables.

The EDA is done in a jupyter notebook called Health_EDA.ipynb


## Task 1:
### Data Loading and Inspection 
In this task, the python libraries were imported as alias.
The data was inspected with the pandas.

## Task 2:
### Handle Misrepresented Data in columns
- Found the ? in the ca column, replace it the mode of the ca column and casted the data type to a float_ 
- Found the ? in the thal column, replace it the mode of the thal column and casted the data type to a float_ 

### Duplicates
*There were no duplicates in the data*


## Task 3:
In Task 3, the heart_disease column was edited to be in 0 and 1 
Where *0* = no heart disease
and *1* = heart disease 

This will make heart_disease column easy to analyze and draw conclusions.


## Task 4:

- The conclusion drawn from this correlation matrix is that, there are low correlation between the age, sex and the heart disease. But there are slightly higher correlation between cp, exang, oldpeak, ca and thal to the heart disease on this a *_conclusion can be drawn that heart disease is more dependent on the lifestyle instead of the age and sex._*

### Pandas CrossTab 
The conclusion draw from the crosstab shown that there is a chance of a male getting a heart disease than a female_

## Task 5:
In the pair plot, we are looking for patterns between the two color groups. Looking at the density plots along the diagonal, there are no features that cleanly separate the groups (age has the most separation). However, looking at the scatterplot for age and thalach (maximum heart rate from an exercise test), there is more clear separation. It appears that patients who are old and have low thalach are more likely to be diagnosed with heart disease than patients who are young and have high thalach. This suggests that we want to make sure both of these features are included in our model.

## Task 6: Communication of Insights

### Significant Predictors of Heart Disease

- Age: Older individuals are at a higher risk for heart disease. The dataset shows a trend where the incidence of heart disease increases with age.
- Sex: Males generally have a higher incidence of heart disease compared to females.
Chest Pain Type (cp): Different types of chest pain (e.g., typical angina, atypical angina) are associated with varying levels of risk.
- Resting Blood Pressure (trestbps): Higher resting blood pressure is linked to an increased risk of heart disease.
- Cholesterol Levels (chol): Elevated cholesterol levels are significant predictors, with higher levels correlating to a greater risk.
- Maximum Heart Rate Achieved (thalach): Lower values in this measurement indicate a higher risk of heart disease.
- Oldpeak: Higher values of oldpeak (depression induced by exercise relative to rest) suggest an increased likelihood of heart disease.
Notable Patterns
- Age Groups: There is a clear pattern where older age groups (e.g., 60 and above) show significantly higher rates of heart disease.
- Gender: Males are more frequently diagnosed with heart disease than females, although the risk for females increases in older age brackets.
