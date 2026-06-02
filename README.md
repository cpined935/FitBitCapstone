# FitBitCapstone

Business Task:
A high-tech manufacturer of women’s health products aims to expand its presence in the global smart device market. Using FitBit Fitness Tracker data from Kaggle, this case study analyzes smart device usage trends, their relevance to the company’s customers, and how they can inform its marketing strategy.

Description of sources:
Data was downloaded from the FitBit Data Fitness Tracker Data on Kaggle and exported as a CSV file to Google Sheets. 

Steps Taken:

Downloaded data from Kaggle: FitBit Data

Selected only columns that would provide insight necessary for this analysis (Calories burned, Total Steps, Sedentary Activity Minutes, Lightly Active Minutes, Fairly Active Minutes, Very Active Minutes). Exported as CSV file. 

Decided to use Google Sheets to import CSV files from Kaggle database. Went through columns to ensure data integrity and that no columns needed to be reformatted before beginning analysis. 

Uploaded cleansed Google Sheet to Posit Cloud using readr() package.

Installed ggplot2 package to create effective and relevant visuals using geom() commands.

There was also some research done on what the specific exercises the categories listed in the database translated to. Both the Mayo Clinic and the Univerity of San Francisco provided necessary clarity in a way that proved to be useful for conducting this analysis. 


Summary: 

One of the most interesting take aways is the fact that more steps taken does not necessarily equate to more calories being burned. The median step count (as shown in the first visual) is also crucial; it shows that the median is almost 2,500 steps below the 10,000 figure that is consistently thrown out as the minimum for the average adult. 


However, there is data missing that would have been very beneficial to the overall analysis. One missing piece is age- an age range would have helped categorize the data into various subgroups. For example, the recommended step count for adults over 60 is between 6,000 and 8,000. If we had the data for age, we could pinpoint what groups are at or below the recommended minimum, and target them with either different ads regarding the importance of getting the minimum steps in daily, or come up with a function for the software to motivate the user to get more steps in (a calendar that gives you a check for everyday you hit the minimum, for example). 

Another very interesting take away from the data is how much lower time spent in the “Fairly Active” and “Very Active” states as opposed to “Sedentary Activity” and “Light Activity”. As shown in the corresponding visuals for each category of activity, the median value for minutes spent in the “Sedentary Activity” category equates to 17.6 hours and the median time spent in the “Light Activity” category equates 3.3 hours- compare those figures to the median time of 6 minutes spent in “Fairly Active” and the 4 minutes spent in the “Very Active” categories and one main question arises: why is that the case? 

Here is where there is more data missing that could be crucial to this analysis, and where a survey could bridge the gap. It would be beneficial to get a better idea of the most common types of activities its users are engaging in and to get a better understanding of how and why consumers are using their products- is it to track workouts, and if so what kind of workouts are they doing? Are they simply using the watch to track certain metrics (heart rate, steps, stress levels, etc.)?

Another aspect that I believe could make this data even more effective is location: where are the bulk of the users? Do they live in heavily populated urban areas (major cities), or do they live in areas that are not as densely populated (towns and suburbs). 

One potential issue with the data that I saw was that for specific time frames (0, 1, 2, 3 minutes) there is a wide range of data for ‘calories burned’. In the Lightly Active pivot table, there are data points that register over 2000 calories burned for 0 minutes of light activity. That does not sound very realistic and it seems like it could either be an error in tracking the duration of the activity accurately or the amount of calories burned accurately. 

*Used median as opposed to average to better take outliers into account.

