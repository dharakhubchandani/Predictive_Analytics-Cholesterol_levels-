# Predictive Analysis of Cholesterol level!
![image](https://github.com/dharakhubchandani/Predictive_Analytics-Cholesterol_levels-/assets/124633398/e682a005-595b-4b15-b3aa-eed12408f3e0)

Dataset: 
Source: https://www.kaggle.com/datasets/thedevastator/exploring-risk-factors-for-cardiovascular-diseas
The dataset is collected from 70,000 individuals. I am aiming to use this dataset to predict the cholesterol level of individuals. The factors included in the study are:
•	Age: age of the respondent (integer)
•	Gender: gender of the respondent (0 = Male, 1 = Female)
•	Height: height of the respondent in centimeters (integer)
•	Weight: weight of the respondent in kilograms (integer)
•	Ap_hi = systolic blood pressure reading of the respondent (integer)
•	Ap_lo = diastolic blood pressure reading of the respondent (integer)
•	Cholesterol = cholesterol level reading as mg/dl on a scale of 0 - 5
•	Gluco = glucose level reading as mmol/l on a scale of 0 – 16
•	Smoke = whether the person smokes or not (0=No, 1=Yes)
•	Alco = whether the person drinks alcohol or not (0=No, 1=Yes)
•	Active = whether the person is physically active or not (0=No, 1=Yes)
•	Cardio = whether the person suffers from cardiovascular disease or not (0=No, 1=Yes)

Data Processing Steps:

1.	Checked if there is any null value for any respondent. There are no null values. 
2.	Added a column for Age in years by dividing the age (integers) by 365 and rounding the number to 2 decimals. 
3.	Dropped the Age (integers) column to avoid duplication. 
4.	Added a column for Gender where there are no numeric values in the column instead it shows Male/Female. When we are creating tables, we do not need 0 or 1 in the output, so I added the column with values Male and Female.
5.	Rename the cholesterol column with ‘cholesterol_levels’

Predictive Analytics: 

Predictive analytics is the process of using data to forecast future outcomes. Generally, the process uses data analysis, machine learning, artificial intelligence, and statistical methods to predict the future outcomes. 

Linear Regression: For predictive analytics, I am using Linear regression method. I am following below steps:
1.	Using the OLS model from statsmodel library to find the variables which are significant in predicting cholesterol levels. 
2.	Creating a regression equation (Y-hat) to be used for statistical calculation of the predicted values. 
3.	Estimating the Cholesterol levels using the regression equation. 


