# Airbnb Price Predictions
Capstone project, presented by Daniella Muhire, Tope Adeolatunji, Orange Xin Lan, Lynette Leiyan Chen and David Lynds  
​
## Overview of the Project
​
When AirBNB launched it was toted as a cheaper alternative to traditional lodging and leisure stays (i.e. hotels accommodations).  Over the years, the price has increased and is increasingly on par or exceeding hotel rates. New York City is one on the most visited cities in North America and has a large number of rentals. With our analysis, we aim to answer the question:
What is an appropriate amount to charge or pay for a rental, based on amenities and location?  Our model will predict this, based on recent market conditions.  


​
## Technology Stack  
To complete this analysis, we are using the following technologies:  
Python (pandas, numpy, geopandas, sklearn among others), Jupyter Notebook, RDS in AWS, and presenting our findings with Tableau.
​
​
In this project, we work with Airbnb listing data for the city of New York. We will take into considerations informations like property type, room type, location, ratings and amenities to predict the price. 
​
Data is current (Sept 7, 2022), and obtained from insideairbnb.com. http://insideairbnb.com/get-the-data/
The dataset we are working with is:
listings.csv.gz
Zip code data was retrieved from https://simplemaps.com/data/us-zips 

​
In the first segment, we clean, organize and perfom exploratory data analysis on our datasets so that they are ready for further in-depth analysis.
​
## Database  
Using RDS service on AWS, we've created our tables and they are ready for input.  From Jupyter Notebook we inserted our data in to the tables using SQLAlchemy.
<img width="953" alt="image" src="https://user-images.githubusercontent.com/104689265/192123941-6328b238-c0cd-4d68-b890-54653c29d35b.png">  

​
## Machine Learning Model Mockup
Since price is a continuous variable, we will use linear regression for our machine learning model. We will use Scikit-learn library, a python machine learning library.The target variable is Price, meaning that the goal of the linear regression model is to predict a price based on some of available features. Database we will use is RDS service in AWS.
​
## Machine Learning
The purpose of this analysis is to utilize Machine Learning statistical algorithms to make predictions based on list prices for Airbnb for New York metropolitan areas. We focused on supervised learning using a free dataset from insiderairbnb.com, which contains datasets of over 39,000 rows and 22 fields for Airbnb property listings in NY metropolitan areas as of September 7th, 2022.

To complete this analysis, we used different Machine Learning techniques, such as linear regression model to train and evaluate the data with four features. These features include zip, bedrooms, minimum_nights and review_score. 

We chose these features because they are all numerical measures, and allow for more meaningful predictions and improve the accuracy score of price for any given listed airbnb property. 

Using the linear modeling approach, we hypotised that certain zips, where heatmaps are concentrated for listed properties will be a good predictor of price because of population density and proximity to city centres such as train stations, shopping centres and restaurants. Example of this is the Upper Eastside and lower Manhattan. Another feature is the review_score, which is positively correlated to list price: the higher the review score, the higher the price. Bedrooms and minimum_nights are also a strong determinant of list price since the more bedrooms and number of nights of stay, the higher the price. We are confident, given the dataset, that the features (dependent variables) above are strong determinant of price (independent variable). 

See sample price prediction below

<img width="953" alt="image" src="https://user-images.githubusercontent.com/104689265/194187352-09694b49-7548-4def-b003-64447e54eb8c.png">

## Individual task:
​
David: Gathered datasets and data cleaning, database set up presentation prep; 
Tope: City Zip Code Clustering, cleaning, machine learning, README.md, presentation prep; 
Lynette: Data Cleaning of listings data, visualizations/dashboards. presentation prep; 
Orange Xin Lan: Data Cleaning of listings data, visualizations/dashboards. presentation prep;
Daniella: Created repository and ReadMe, machine learning, presentation prep.

## Presentation

Deck

https://docs.google.com/presentation/d/1R67jjSp2edGHn62J34kEa3NTQhn0paBVsokQ9WaNDl0/edit?usp=sharing_eil_m&invite=CPDLx4oH&ts=6332253a

