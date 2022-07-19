# Airplane-Crash-Report 

**INTRODUCTION**

The dataset contains data of airplane accidents involving civil, commercial, and military transport worldwide from 1908-09-17 to 2009-06-08. It provides information about the history of airplane crashes around the world, the causes, and the death rates.

# PROBLEM STATEMENT

Airplane crash leads to loss of lives and most of the survivors do live with the negative effects e.g trauma, diabilities etc. it had on them for the rest of their lives. This project hope to enable the readers to know what to do in order prevent airplane crash in the future and give them insights on previous occurrences including the rate of fatality and survival etc.

# PROBLEM OBJECTIVES

The goal of this project is to provide insights on and provide answers to the following questions:

* Which Country has the highest fatality rate?

* What is the rate of Fatality and Survival?

* What is the type of airplane with the highest occurrence of fatalities and survivals?

* When did the most fatal airplane crash happen? WHat is the number of fatalities and where did it take place?

* Which year has the highest number of Survivors and which one has the highest number of Fatalities yearly?

* What is the record of the number of survivors and fatalities monthly?

* Compare the sum of passengers aboard, fatalities and survivors by operators including the survival and fatality rates.

# DATA SOURCING

This data was provided by Mr. Oyinbooke Olanrewaju @theoyinbooke after the completion of the 30 days of learning programme. The link to the data is provided below;

https://raw.githubusercontent.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/main/Airline%20Project/Airplane_Crashes_and_Fatalities_Since_1908.csv

The data is imported as a CSV file to Excel from web by clicking on **Get Data** under data tab, click on other sources and then from WEB.
![DaTransform 002](https://user-images.githubusercontent.com/102861459/179799842-d05d78c2-ff7d-4642-ac6c-36c285e5dcda.png)

# DATA TRANSFORAMTION

After the data was imported into Excel from web, it was then transformed using Power query. Exploration and Observation of the dataset was done in order to know the state of the dataset and since it was found to be dirty, I started with cleaning the data by ensuring it is correct, completely free of errors, outliers and special characters.I also checked for duplicates and changed each variable to their appropriate data type.

Using text after delimiter function in Power Query(Excel), I extracted the countries from Location and I noticed that they mostly included states instead of countries especially for USA, also spelling mistakes, repetitive words and rearrangement of letters of other countries. For the states in USA I replaced them with USA for the sake of uniformity and easy visualisation and storytelling and it was done by right-clicking on the column that consists of the states and select replace values, each states are replaced with USA.

In each of the columns; for Variables whose data type is Text, blank rows or null rows are replace with Unknown while for variables whose data type is number, blank rows or null are replaced with 0

# FURTHER ANALYSIS USING POWER BI

Imported the dataset into Power BI, using Power query made some modifications:
* made use of clean and trim under format option in the transform tab to clean and trim the variable in order to ensure uniformity,
* realized that some special characters were still present, used “replace values” to remove them.

After loading the data into Power BI, further analysis were carried out:
1. Created measures for the required parameters I needed: such as Total fatalities, total passengers aboard, survival rate, fatality rate etc.
2. created a new table which served as the Date table and added Year, month, monthnumber etc. columns
3. established a relationship between the airplane crashes and fatalities table and date table using Data Modeling

# DATA VISUALIZATION
The choice of colour was to lay emphasis on the subject matter and the story

**KEYWORDS**
•	Date - Date of accident
•	Time - Local time, in 12 hr. in the format hh:mm:ss
•	Location - Location of the accident
•	Operator - Airline or operator of the aircraft
•	Flight - Flight number assigned by the aircraft operator
•	Route - Complete or partial route flown prior to the accident
•	Type - Aircraft type
•	Registration - ICAO registration of the aircraft
•	cn/In - Construction or serial number / Line or fuselage number
•	Total Aboard - Total people aboard
•	Passengers Aboard - Passengers aboard
•	Crew Aboard - Crew aboard
•	Total Fatalities - Total fatalities
•	Passengers Fatalities - Passengers fatalities
•	Crew Fatalities - Crew fatalities
•	Ground - Total killed on the ground
•	Summary - Brief description of the accident and cause if known

# RECOMMENDATION
From the research and analysis carried out during the course of the project, the following are recommended;
1. It is advisable that the avaiation control house and the pilots work together so as to prevent airplane crash and also save lives.
2. Proper maintenance of the aircraft and constant check should be carried out before making use of the aircraft for transportation.
3. During trainings novice or beginners should be properly monitored when training.
4. Though weather conditions can be unpredictable sometimes, it is advisable that the weather and climate station to be atleast 99.98% sure of the weather conditons before the aircrafts take off. 
