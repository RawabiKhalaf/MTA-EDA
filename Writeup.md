# Exploratory Data Analysis Project - NYC Self-Driving Taxis Distribution Plan
Rawabi Alharbi

## Abstract
The goal of this project was to ...      

## Design
The New York City Taxi and Limousine Commission (TLC) is an agency that is responsible for licensing and regulating New York City's taxi cabs. For the last four years, TLC has been working on making 5000 self-driving taxis to start officially distributing them in late 2022. But as a first step, They are planning to test 50 self-driving taxis at 5 different subway stations that are the nearest to a park since these test taxis are going to be able to only take the passenger from the station to the nearest park to ensure passengers safety of a short ride through this testing experience. In addition, this test is going to take place on one of the last three months of 2021, three days per week. Therefore, they need to decide the distribution plan based on the highest number of registered exits per station near the park, the highest number of registered exits per station per month, and the average total number of registered exits per weekday.

## Data
The MTA data which contains partainign the turnstile gate for each station.  The dataset is a series of data files containing numbers of cumulative entries and exits by stations, turnstile, along with their dates and time. The data records are weekly produced and mostly collected every 4 hours. The data sample I've chosen is the last three months of 2019. The sample includes 2474417 rows and 11 columns.

## Algorithms
* Data cleaning:
  1. Fixing the reverse counter problem
  2. Dealing with outliers with the help of quantiles
  3. Adding boolen column PARK which checks if station is neer to a park or not based on the station's name
  4. Adding other columns needed for exploring the data:
      * DATE_TIME column
      * MONTH column
      * DAY column

* Data validation:
  1. Checking no nulls
  2. Checking no duplicates
  3. Fixing turnstiles issue

* Methodology of exploring the data:
The data was filtered based on the stations that are neer to any park, then the average total number of registered exits was calculated for each.
The average total number of registered exits was calculated also for each of the filtered stations for each month. As a last calculation, the average total number of registered exits was taken for each day of the week in order to find the hieghst three week days.

## Tools
- Python and Jupyter Notebook
- Numpy and Pandas for data manipulation
- Matplotlib and Seaborn for plotting visuialization
- SQLAlchony and SQLite for importing, exporting, storing and exploring the data.

## Communication
<img width="423" alt="image" src="https://user-images.githubusercontent.com/87195262/135451326-0885b08b-4fa0-4a19-93d3-54a48736e7dd.png">
<img width="306" alt="image" src="https://user-images.githubusercontent.com/87195262/135451335-dd7a51fe-71a1-430d-b04f-352f8f141de9.png">
<img width="363" alt="image" src="https://user-images.githubusercontent.com/87195262/135451344-74edccb4-2749-4089-8262-85b911859b1d.png">
