# Flight_Fare-Prediction
Main aim of the project is to determine the price of flight based 
on some features like Airline, Source, destination, Route , Duration, Departure time, Arrival time. 
Data Cleaning;Dropping missing values (just two missing values), extracted day and month data from Date_of_journey, extraction of hours and minutes from departure,arrival time and also duration and drop corresponding columns.
Exploratory Data Analysis: cat plot of the different Airlines against Price, also source against price
Feature Engineering: One hot encoding for the columns(Airline, destination and route), dropping route because it is related to the Total_stops thereby eliminatinating redundancy, drop Additional info column (contains 80 percent garbage), label encoding for the nominal variable (Total_stops), concatenation of the onehot encoded columns with the training dataset
Feature selection: using perason correlation( no columns were really more than 90 percent correlated), using extra tree regressor and callig feature_importances_ attributes 
Data Split 
model fit using Random Forest Regresssor
model evaluation using MAE,MSE, RMSE, R2_score
Hyperparameter optimization using RandomizedSearch CV
