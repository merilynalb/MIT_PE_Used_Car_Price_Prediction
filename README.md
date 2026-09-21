# MIT PE Capstone Project: Used Car Price Prediction
As part of MIT Professional Education's Applied AI and Data Science Program, this coursework explored the Indian Used Car Price dataset and used various supervised machine learning regression tools to predict prices based on key features identified.

## Overview of the project
The objective of this project was to predict the price of pre-owned cars in the Indian car market to help a tech start-up improve their pricing strategies. To understand the dataset, EDA was used to explore the features and identify correlations between the dependent and independent variables. The dataset was subsequently tidied for skewness, missing values, outliers and prepared for regression modeling. Various models (linear algorithms: OLS and Ridge regression, and non-linear algorithms: Decision Trees and Random Forests) were systematically tested to predict used car price on the training datasets, with iterations performed to improve prediction scores (R2, RMSE). Each model was tested on unseen dataset and final model performance was evaluated. 

## Key Highlights
- Using EDA to gain insights from the features
- Data preprocessing and preparation for regression modeling
- Building and iteratively improving the linear (OLS, Ridge regression) and non-linear (Decision Trees, Random Forests) regression models
- Evaluating model performance using key metrics (R2, RMSE, multicollinearity) and comparing performance against other models
- Evaluating if the model over/under-fits the training data using 10-fold cross-validation
- Testing the model on unseen data
- Summary of recommendations to the buisness

## Dataset
Each record in the dataset represents a used car in the Indian car market. Detailed attribute information can be found below:

Attribute information:
- S.No. : Serial Number
- Name : Name of the car which includes Brand name and Model name
- Location : The location in which the car is being sold or is available for purchase (Cities)
- Year : Manufacturing year of the car
- Kilometers_driven : The total kilometers driven in the car by the previous owner(s) in KM
- Fuel_Type : The type of fuel used by the car (Petrol, Diesel, Electric, CNG, LPG)
- Transmission : The type of transmission used by the car (Automatic / Manual)
- Owner : Type of ownership
- Mileage : The standard mileage offered by the car company in kmpl or km/kg
- Engine : The displacement volume of the engine in CC
- Power : The maximum power of the engine in bhp
- Seats : The number of seats in the car
- New_Price : The price of a new car of the same model in INR 100,000
- Price : The price of the used car in INR 100,000

## File Summary
This project contains three files:

used_cards.csv: The Indian Used Car dataset
Capstone_Project_Reference_Notebook_Full_Code_Used_Cars_Price_Prediction_MMA.ipynb: The Jupyter notebook
Capstone_Project_Reference_Notebook_Full_Code_Used_Cars_Price_Prediction_MMA.html: The HTML file to visualise the code and figures easily

## Libraries Used
This project used the following libraries in Python:

For general use and data tidying:
- numpy
- pandas

For visualisation:
- seaborn
- matplotlib

For regression modeling:
- statsmodel
- scikit-learn

## Conclusion
Our comparisons highlighted that OLS Model 3 performed the best, with the highest R2 value of 0.93 and lowest RMSE value of 0.20. It out-performed other linear and non-linear models, and highlighted Power and Year as the two most influential features that help predict used car prices. 

No model could accurately predict used cars above INR 4,000,000 due to the low number of data points available above this threshold. Thus, it is recommended to use OLS Model 3 to predict used car prices up to this threshold, until further data points can be gathered to improve prediction performance for more expensive used cars. 

## Grading
TBD
