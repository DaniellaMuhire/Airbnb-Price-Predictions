# Airbnb Price Predictions
Capstone project, presented by Daniella Muhire, Tope Adeolatunji, Orange Xin Lan, Lynette Leiyan Chen  
​
## Overview of the Project
​
There has been conversation on social media and in the news about AirBNB as of late.  When AirBNB launched it was toted as a cheaper alternative to traditional Lodging and leisure stays (i.e. hotels accommodations).  Over the years, the price has increased and is increasingly on par or exceeding hotel rates. New York City is one on the most visited cities in North America and has a large number of rentals. With our analysis, we aim to answer the question:  
-What will AirBNB rates look like in a year? 2 years?
​
## Communications Protocol  
Our group maintains communication through Slack, Zoom, Class Breakout rooms, and shares our work and ideas via Github through our shared repository.
​
## Technology Stack  
To complete this analysis, we are using the following technologies:  
Python (pandas, numpy, geopandas, sklearn among others), Jupyter Notebook, RDS in AWS, and presenting our findings with JavaScript, HTML, CSS, Flask.
​
​
In this project, we work with Airbnb listing data for the city of New York. We will take into considerations informations like property type, room type, location, ratings and seasonality to predict the price. 
​
Data is current (Sept 7, 2022), and obtained from insideairbnb.com. http://insideairbnb.com/get-the-data/
The two datasets we are working with are:
listings.csv.gz
calendar.csv.gz
​
In this first part, we clean, organize and perfom exploratory data analysis on our datasets so that they are ready for analysis.
​
## Database  
Using RDS service on AWS, we've created our frames and ready for input.  
<img width="953" alt="image" src="https://user-images.githubusercontent.com/104689265/192123941-6328b238-c0cd-4d68-b890-54653c29d35b.png">
​
## Machine Learning Model Mockup
Since price is a continuous variable, we will use linear regression for our machine learning model. We will use Scikit-learn library, a python machine learning library.The target variable is Price, meaning that the goal of the linear regression model is to predict a price based on some of available features. Database we will use is RDS service in AWS.
​
## Machine Learning
The purpose of this analysis is to utilize Machine Learning statistical algorithms to make predictions based on list prices for Airbnb for New York metropolitan areas. We focused on supervised learning using a free dataset from insiderairbnb.com, which contains datasets of over 39,000 rows and 22 fields for Airbnb property listings in NY metropolitan areas as of September 7th, 2022.

To complete this analysis, we used Linear Regression Machine Learning model to train and evaluate the data with numerical features in the dataset. 

First of all, we find which feature has a relationship with the target, Price. After analyzing different features from the dataset as indepedent variables and Price as the depedent variables, we realised that only Minimum_nights, Number of Reviews and review scores has a relationship with the target. 
We also found that the relationship is weak.

<img width="983" alt="Minimum_nights" src="https://user-images.githubusercontent.com/77806210/194414319-ecdbd7c0-60f7-4484-b03e-99e6a2bed6ff.png">
<img width="1196" alt="Number of Reviews" src="https://user-images.githubusercontent.com/77806210/194414356-7a399f42-59e4-4b5a-b728-3a88f2ce994a.png">
<img width="1180" alt="Review Scores" src="https://user-images.githubusercontent.com/77806210/194414433-ef17bdf9-597a-4b98-977e-e5995bda2061.png">

For the model, we used minimum_nights to predict the price. We fit and trained the model on that feature. We also found the coefficient and intercept of the model. 

## Individual task:
​
David: Gathered datasets and data cleaning of calendar data, database set up; 
Tope: City Zip Code Clustering; 
Lynette: Data Cleaning of listings data; 
Orange Xin Lan: Data Cleaning of listings data; 
Daniella: Created repository and ReadMe

## Presentation

Deck

https://docs.google.com/presentation/d/1R67jjSp2edGHn62J34kEa3NTQhn0paBVsokQ9WaNDl0/edit?usp=sharing_eil_m&invite=CPDLx4oH&ts=6332253a

