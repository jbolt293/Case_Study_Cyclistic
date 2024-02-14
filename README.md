# Google Data Analytics Case Study 1: Cyclistic Bike Share
## Introduction
This case study will present the culmination of every lesson that I've learned whilst completing the Google Data Analytics certificate program. I will use these skills to complete a case study for a fictional bike-share company named Cyclistic. I will help the company make data-driven decisions on how they can increase the amount of customers that sign up for annual memberships by using the data analysis process of Ask, Prepare, Process, Analyze, Share, and Act. 
## Ask
### Question at Hand:
How do annual members and casual riders use Cyclistic bikes differently?
### Key Stakeholders
* Lily Moreno: The director of marketing at Cyclistic and my manager. She is responsible for the development of initiatives for promoting the bike-share program.
* Cyclistic Marketing Analytics Team: A team of data analysts who are responsible for collecting, analyzing, and reporting data that helps aid Cyclistic's marketing strategy.
* Cyclistic Executive Team: The notoriously detail-oriented team that decides whether to approve the new marketing program or not.
## Prepare
The first step I completed in preparation for my analysis was to download all the data that was necessary. I downloaded the Cyclistic Trip Data from 2022 to see how customers accessed and used the bike-share. To do this, I had to download all 12 .csv files and store them in their dedicated folders. The data used was provided by Motivational International Inc. with a liscense that can be found [here](https://divvybikes.com/data-license-agreement). 
## Process
I decided to use R in order to clean the data and analyze it. To do this, I went onto RStudio and first installed any packages that I needed for this case.  and loaded all of the datasets onto it. In order to do this, I had to use the "read_csv" fucntion from tidyverse
When all of the datasets were loaded into BigQuery, I combined all of them into a single dataset I labeled as "Combined_Divvy_TripData" by using the __UNION__ function. I then removed any rows of data that contained values that were null by using the __DELETE FROM__ function. After doing this, I removed any duplicates from the dataset by using the __SELECT DISTINCT__ function and saved it as another dataset. 

Now that the data has been properly cleaned. I need to visualize it. In order to do this, I decided to use R. By importing the cleaned dataset into RStudio (Posit Cloud), I was able to visualize the data. I did have to fine-tune the dataset before doing this, as RStudio had changed the column names of the dataset. I used the __names()__ function to change the names back to their original state. I then had to remove the row in which the original names of the columns were moved to. To do this, I input a line of code, being 'Cleaned_Divvy_TripData = Cleaned_Divvy_TripData[-1,]' 
## Analyze
Now that I have cleaned up the data using SQL and have imported the dataset into RStudio, I am able to analyze the data and see what trends there are in order to formulate ideas on how to answer the question at hand.
