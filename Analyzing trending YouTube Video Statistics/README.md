# Analyzing trending YouTube Video Statistics

## Objective
YouTube (the world-famous video sharing website) maintains a list of the top trending videos on the platform.
According to Variety magazine, “To determine the year’s top-trending videos, YouTube uses a combination of factors including measuring users interactions (number of views, countries, categories, comments and likes).  
In this project, we want to analyze the various factors that affect the popularity of videos and also study relationships between these youtube video parameters.

## Motivation
Predicting factors that could make a video popular can help advertisement companies for making investments for certain videos.  
It can also help bloggers in knowing the aspects in a video that could increase their views.  
We wish to mine the various interactions between parameter to provide an insight of how popularity of videos is affected by region or their category.

## Data Set
We have leveraged the data set available on Kaggle.com.The data was collected using you tube API.  
This dataset is a daily record of the top trending YouTube videos from Nov 2017 - April 2018.  
Data is available for 6 countries: Canada, Germany, France, Great Britain, United States.  
The data is available in two formats i.e CSV & JSON files. JSON file contains data pertaining to video categories.  
No. of total data records: 130,712 

Below is the link for data set: https://www.kaggle.com/datasnaek/youtube-new/data

#### Response Variable: 
Views- Number of views   

#### Possible Predictor:  
Likes: Number of likes   
Dislikes: Number of Dislikes   
Comment_count : Number of Comments   
Publish Date: Date on which video was published.   
Trending Date: Dates on which a particular video was trending.   
Category : The category to which a video belongs. (15 Categories)   
Trending days: Number of days a video was trending (Derived column)

Please read the report for the detailed exploratory analysis.
