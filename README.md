# Airbnb Price Predictions
Capstone project, presented by Daniella Muhire, Tope Adeolatunji, Orange Xin Lan, Lynette Leiyan Chen  
​
## Overview of the Project
​
There has been conversation on social media and in the news about AirBNB as of late.  When AirBNB launched it was toted as a cheaper alternative to traditional accommodations.  Over the years, the price has increased and is increasingly on par or exceeding hotel rates. New York City is one on the most visited cities in North America and has a large number of rentals. With our analysis, we aim to answer the question:  
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
![Getting Started](./database.png)
​
## Machine Learning Model Mockup
Since price is a continuous variable, we will use linear regression for our machine learning model. We will use Scikit-learn library, a python machine learning library.The target variable is Price, meaning that the goal of the linear regression model is to predict a price based on some of available features. Database we will use is RDS service in AWS.
​
## Individual task:
​
David: Gathered datasets and data cleaning of calendar data, database set up; 
Tope: City Zip Code Clustering; 
Lynette: Data Cleaning of listings data; 
Orange Xin Lan: Data Cleaning of listings data; 
Daniella: Created repository and ReadMe
