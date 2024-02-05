# Airline-Passenger-Satisfaction

## Objective
The aim of this project is to assist an airline company in identifying the key factors that impact customer satisfaction. Customer satisfaction significantly influences a company's business outcomes, making it crucial to analyze and enhance the factors closely linked to it for sustainable growth and a positive reputation.

Following the CRISP-DM methodology, this project progresses through six phases: Business Understanding, Data Understanding, Data Preparation, Data Modeling, Evaluation, and Deployment.

## About the Data Set

The dataset for this project is obtained from Kaggle which contains the data sourced from a survey conducted by airlines on the satisfaction level of passengers/customers based on various factors. The dataset consists of 25 columns such as Age, Gender, Travel class, Arrival and Departure delays. Also, it features that influence customer satisfaction levels such as On-board service, Cleanliness, Seat comfort, Baggage handling etc.
The dataset consists of a column or feature named ‘satisfaction’ which describes the overall satisfaction level of the customer. It has two values, ‘neutral or dissatisfied’ and ‘satisfied’. This satisfaction feature is considered as the label feature since it conveys the overall experience of the customer based on the ratings given for other features. The dataset consists of 103904 and 25976 records in train and test respectively.

## Data Cleaning and Visualization

Data cleaning plays a key role in deriving the output of a machine learning model. Usually, data cleaning consists of processes like determining outliers and removing or imputing outliers, removing or replacing missing values, removing duplicate values, and removing values with less or no importance.
In this project, the ‘Arrival Delay in Minutes’ column has 310 missing values. These missing values are imputed with the mean values of the non-missing values of the same column.
Data Visualization plays an important role in understanding the data as it gives an overview of the data before the model implementation. Exploratory Data Analysis is done for the dataset.

## Feature Selection

We use the Lasso Regression path to understand the correlation between features and the target variable, which is our 'satisfaction column. We observe that ‘Gender, ‘Food and Drink’, ‘Age’, 
‘Flight Distance’, ‘Departure.Delay.in.Minutes’, and ‘Gate Location’  are the columns’  whose coefficient becomes 0 when lambda increases. Thus we exclude these columns. Now we proceed with the remaining columns toward model fitting

## Model Selection

We use two models as part of the comparative study:

#### Random Forest
#### Logistic Regression

## Conclusion

We observe that Random Forest performs better compared to Logistic Regression, in every metrics
Metrics : 
Logistic Regression	

Accuracy - 0.8692	

F1 Score - 0.8451	

Recall - 0.8297	

Precision - 0.9013	

Kappa - 0.7321
Random Forest	

Accuracy - 0.9790

F1 Score - 0.9817

Recall - 0.9897

Precision - 0.9651

Kappa - 0.9573







