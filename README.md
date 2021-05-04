# Nigeria-COVID-19-Data-Analysis-Using-Python

Ustacky Data Scientist Microdegree Capstone Project


# Project Overview

Coronavirus disease (COVID-19) is an infectious disease caused by a newly discovered coronavirus, and it has affected major parts of the world. Nigeria, a West-African country, has also been affected by the COVID-19 pandemic after recording its first case on 27th February 2020.

Nigeria is a country with 37 states - Federal Capital Territory included- and a fast-growing economic environment with about 200 million citizens. COVID-19 has affected several country activities as the country steadily progressed from its first case to shutting down major airports, state-wide lockdown, curfews, and reviving its economy.

In this project, data science & analytics skills are being employed to collect data, explore the data, perform analysis, create visualizations, and generate insights.


# Steps/Approaches

STEP 1: Data Collection - Different data is collected from different sources and combined to perform analysis and provide insights. 
- From NCDC COVID-19 official website, the data is obtained by performing a web extraction/web scrape
- The Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE) daily data is read in using Pandas from its GitHub repository
- Nigeria Community Vulnerability Index data, Real Domestic Gross Product Data and State Budget Data is downloded and read in from current working directory
- Another external data from Our world in data [website](https://ourworldindata.org/coronavirus/country/nigeria) for COVID cases in the world is downloaded and read in also. 

STEP 2: View the Data - Basic information about all the data using the head(), shape and info() method were obtained. All data showed no missing value and were in their appropriate datatype except the ncdc scraped data.

STEPP 3: Data Cleaning & Preparation - From the information obtained above, there is need to fix the data format of the scraped dataframe. The numerical columns are converted to appropriate data type; integer and comma(,) removed. Columns of the scraped data are renamed. Daily data for Nigeria is extracted from the Global daily cases data.

STEP 4: Data Analysis - Here, some analysis on the datasets are performed and findings communicated  in charts and summarised. A few analysis carried out include:
1. A plot of the top 10 states in terms of Confirmed Covid cases by Laboratory test, Discharged Covid cases, cases on admission and Death cases
2. Line plot for the total daily confirmed, recovered and death cases in Nigeria
3. Line plot of the daily infection rate in Nigeria
4. The maximum infection rate for a day in Nigeria and the date
5. The relationship between the external dataset and the NCDC COVID-19 dataset is determined by combining the two dataset together on a common column(states), then a a line plot of top 10 confirmed cases and the overall community vulnerability index on the same axis generated.
6. A regression plot between two variables Confirmed Cases and Population Density to visualize the linear relationships
7. A barplot using the GDP values for each year & quarters from the Real GDP Data
8. Further analysis was carried out on more external dataset. Plot of the initial and revised budgets, plot of the number of lab confirmed cases and the number of death according to their regions 
9. Visulaizations on the owid datest to answer more question like: the total cases for years 2020 and 2021 in Nigeria, Plot of the total death per month and new cases per day. 
10. Plot of the number of people vaccinated each month and record of the total tests of both years in Nigeria.


# Insights

Some insights discovered from the analysis of the COVID cases in Nigeria is listed below. Check out the Executive summary above for better explanation and the visuals.
1. Lagos is the top state with confirmed COVID cases by laboratory test
2. The maximum infection rate is about 2464
3. The fourth quartile in 2020 is at 0
4. The South west has the higest number of laboratory confirmed cases. Also, leading with over 400 deaths cases, follwed by the South south, North central, North west, North east and then South east regions
5. April holds the record of most vaccinated people


# Suggestions on future work/Improvement plans

Importation of more COVID datasets for better comparison and more diverse analysis. Also, Build a machine learning model to predict rate of new cases, death etc. in Nigeria.