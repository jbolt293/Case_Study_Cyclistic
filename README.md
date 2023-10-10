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
The first step I completed in preparation for my analysis was to download all the data that was necessary. I downloaded the Cyclistic Trip Data from 2022 and 2023 to see how customers accessed and used the bike-share. To do this, I had to download all 19 .csv files and store them in their dedicated folders. The data used was provided by Motivational International Inc. with a liscense that can be found [here](https://divvybikes.com/data-license-agreement). 
## Process
I decided to use SQL in order to clean the data and analyze it. To do this, I went onto BigQuery and loaded all of the datasets onto it. Since some of the .csv files were over 100mb, they could not be loaded into Bigquery by just uploading them. So to bypass this, I made a bucket on Google Cloud Storage and put any files over 100mb into the bucket so they could be loaded into BigQuery.

When all of the datasets were loaded into BigQuery, I combined all of them into a single dataset I labeled as "Combined_Divvy_TripData" by using the __UNION__ function. I then removed any rows of data that contained values that were null by using the __DELETE FROM__ function. After doing this, I removed any duplicates from the dataset by using the __SELECT DISTINCT__ function and saved it as another dataset. 
