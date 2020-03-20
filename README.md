# FinalProject
Final Project

1)  Research question:   We will analyse data for US traffic accidents. Our analysis with take into account various factors which might have lead to an accident. We will look into severity , number of accidents, visibility, road condition , time and other factors that might have lead to an accident. We will predict what conditions often leads to an accident and also its severity. Our model will help general population to understand underlying factors that might lead to an accident and get a better understanding.
2)  Domain and Data: 
    Source of Data - https://www.kaggle.com/sobhanmoosavi/us-accidents
    Domain - Law, geospatial analysis, 

      a)  preprocessing that may be necessary: 
          Check for missing values, Handle Null values, Manage categorical data, Handle noisy data, Check for outliers, feature                   engineering.

      b)  size of data :
          US_accidents.csv - 3M records with 49 columns

      c)  tentative plan for analysis on GCP

           1)  EDA and Preprocessing:
               a. Number of accidents per state, county, zipcode
               b. Find correlation between different natural factors
               c. Time of day which has most accidents
               d. Severity of accidents
               e. State wise length of road affected by an accident
               We can directly work on the preprocessed data and implement the recommendation algorithm.

           2)  Dashboard for User group, Dashboard for Data Engineers:
               We will plan to represent graphically the severity of accidents. Also dashboards for the accidents occured based on                      various factors.
           3)  GCP further processing :
               We will use classiffication algorithms(KNN, Random Forest , decision tree) to predict the severity of an accidents

           4)  Evaluation of results :
               We will be evaluating our result by RMSE(Root Mean Square Error) and AUC. The smaller the value more accurate result will                be. We will try to implement and tune the algorithm to get the least RMSE.          

           5)  Steps for production model :
               We will load our data in Classification model and train our model with partial data and check RMSE . After training , we                will be testing our model and prepare the model for Production data.

           6)  Final Dashboard for User Group :
               Finally, we can recommend users the chances of accidents and severity based on various factors . This will help users                    plan a trip better, we will do this by finding the conditions that make travel risky
