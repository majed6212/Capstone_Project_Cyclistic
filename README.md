# Capstone Project Cyclistic
Google Data Analytics Professional Certificate Capstone Project - Cyclistic Dataset

This repository shows my analysis of the Cyclistic capstone project as part of completing Google Data Analytics Professional Course.<br>

This project is divided into 2 sections:<br>
- The data preparation/processing/analysis is done using ***Power Query***.<br>
- The data visualization is done via ***Power BI***, the final report can be found in report.pdf which was produced using ***Power Bi***.

#### Table of content
- The scenario
- Ask
- Prepare
- Process
- Analyse
- Share
- Act<br>
### The Scenario:

As a junior data analyst in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, the team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve my recommendations, so they must be backed up with compelling data insights and professional data visualizations."

#### About the Company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geo-tracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.

#### Deliverables:
- A clear statement of the business task
- A description of all data sources used
- Documentation of any cleaning or manipulation of data
- A summary of the analysis
- Supporting visualizations and key findings
- Top three recommendations
- Ask

> #### Identify the business task
> The future success of the company depends on the conversion of casual riders to annual memberships.<br> The purpose of this analysis is therefore to discover the key >differences in the use of rental bikes by 2 different users of the bikes: <br> 
> - Annual members.<br>
> - Casual riders.

> #### Statement of the business task:<br>
> How do annual members and casual riders use rental bikes differently?

> #### Key stakeholders:<br>
>Cyclistic executive team, Director of Marketing (Lily Moreno), Marketing Analytics team.

### Prepare
Gathering the datasets for the year 2021<br>
Description of the datasets:<br>
Preparing the datasets<br>
Verifying the credibility of the data:<br>

> To proceed with the next steps of this analysis the excel files are uploaded to ***Power Query***:


### Process
Combining the uploaded 12 CSV files into 1 CSV using Power Query editor

#### Steps in power query:

- Adding; extracting new columns such as `trip_duration` by subtracting the `ended_at` column from `starting_at` column, name of the day, month from `starting_date` column for aggregation and more appealing viz.
- Replace empty cells with Not Available in `start_station_name` and `end_station_name` to find the most visited station and count the most completed trip that occurred using a single column, i.e. 'From Menard Ave & North Ave to Bloomingdale Ave & Harlem Ave'.
- Combine the start station name and end station name into a new feature called trip which will be used to count the number of trips and average time per trip.
- Concatenate all 12 files from Jan 2021 to Dec 2021 into one file containing 5.9M rows after performing all the steps above.
- Rename the last column from ‘member_casual’ to customer.

#### Steps in power bi:
- Visualization.
- Report.
- Dashboard


#### Finding other irregularities within the dataset

Converting any negative value in column `trip_duration` to positive, this was found after creating `trip_duration` column, since I don't have access to the data author I decided the following:<br>
I assumed that this was a mistake and took the absolute of the number since it is impossible to have a negative value for a trip.


### Analysis
Conducting descriptive analysis<br>
A descriptive analysis of the new `trip_duration` (in minutes)

#### Comparing members and casual users
The average ride time per day for members vs. casual users.<br>
The correctly ordered day of the week average ride time per day for members vs. casual users.<br>
Analysis of the ridership data by type and weekday

### Share


Number of rides for members and casuals<br>
The average duration of trips

Exporting this dataset to ***Power bi*** and downloading it into my machine as a CSV file using an external tool ***DAX-studio*** to perform the analysis.
