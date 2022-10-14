# Airbnb Price Predictions
Capstone project, presented by Daniella Muhire, Tope Adeolatunji, Orange Xin Lan, Lynette Leiyan Chen, David Lynds.
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
In this project, we work with Airbnb listing data for the city of New York. 
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
Since price is a continuous variable, we will use Supervised Learning regression model's algorithms for our machine learning models. We will use Scikit-learn library, a python machine learning library.The target variable is Price, meaning that the goal of the models will be to predict a price based on some of available features. Database we will use is RDS service in AWS.
​
## Machine Learning
The purpose of this analysis is to utilize Machine Learning statistical algorithms to make predictions based on list prices for Airbnb for New York metropolitan areas. We focused on supervised learning using a free dataset from insiderairbnb.com, which contains datasets of over 39,000 rows and 22 fields for Airbnb property listings in NY metropolitan areas as of September 7th, 2022.

To complete this analysis, we used three different regression model's algorithms, such as linear regression model, random forest regressor and Decision tree Regressor. With these algorithms, we analyze the data and attempt to identify patterns. Based on these patterns, the model makes predictions on new data.

We assess the performance of each regression model with the standard metric called Root Mean Squared Error or RMSE.

The linear regression model has a RMSE of 0,238.
<img width="1359" alt="Linear Regression Model" src="https://user-images.githubusercontent.com/77806210/195737700-e597fc48-3061-46c1-b096-edfa28c63f64.png">

The Random Forest Regressor model has a RMSE of 0,226.
<img width="1299" alt="Random Forest Regressor" src="https://user-images.githubusercontent.com/77806210/195737674-32e5ea00-18c1-41de-8b99-62dbb1ce3926.png">

The Decision Tree Regressor model has a RMSE of 0,304.
<img width="1230" alt="Decision Tree Regressor" src="https://user-images.githubusercontent.com/77806210/195737646-4828e330-3370-42b6-ad10-c833135bed34.png">


We know that the lower the RMSE, the better the model. We can therefore conclude that the Random Forest Regressor model is a better fit to predict the price because of its low RMSE.

## Individual task:
​
David: Gathered datasets and data cleaning of calendar data, database set up; 
Tope: City Zip Code Clustering; 
Lynette: Data Cleaning of listings data; 
Orange Xin Lan: Data Cleaning of listings data; 
Daniella: Created repository, contributed to ReadMe and  did Machine Learning file. 

## Presentation

Deck

https://docs.google.com/presentation/d/1R67jjSp2edGHn62J34kEa3NTQhn0paBVsokQ9WaNDl0/edit?usp=sharing_eil_m&invite=CPDLx4oH&ts=6332253a

Tableau Story

https://public.tableau.com/app/profile/lynette.chen/viz/AirbnbStory_16654366921700/AirbnbStory


