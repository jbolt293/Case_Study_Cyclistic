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

I decided to use R for this case study. To do this, I went onto RStudio and first installed any packages that I needed for this case. The code for that can be found [here](https://github.com/jbolt293/Case_Study_Cyclistic/blob/main/Install%20Packages). After installing all of the necessary packages, I loaded all of the datasets from 2022 onto it. The code for that can be found [here](https://github.com/jbolt293/Case_Study_Cyclistic/blob/main/Add%20Data%20to%20RStudio). In order to do this, I had to use the __read_csv__ function from tidyverse. After loading all of the data into RStudio, I combined all of the datasets into one big dataset using the __bind_rows__ function. the code for that can be found [here](https://github.com/jbolt293/Case_Study_Cyclistic/blob/main/Bind%20all%20Datasets%20into%20One).
## Process
Now that everything has been prepared for the process phase, including installing packages and loading datasets, I can begin to process the data. The first step I took was to add more columns into the dataset. Those being columns for date, month, year, and day of week columns. To do this, I had to imput the code chunk which can be found [here](https://github.com/jbolt293/Case_Study_Cyclistic/blob/main/Add%20date%2C%20month%2C%20year%2C%20and%20day%20of%20week%20columns). Then, I had to convert the column __ride_length__ to numeric for calculation purposes. The code for that can be found [here](https://github.com/jbolt293/Case_Study_Cyclistic/blob/main/Convert%20ride_length%20to%20numeric). 

## Analyze

