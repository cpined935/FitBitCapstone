# FitBitCapstone

**Business Task:**
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


<img width="470" height="270" alt="image" src="https://github.com/user-attachments/assets/0df3fd80-d3c7-43e4-b000-928a02cd5abd" />

<img width="470" height="270" alt="image" src="https://github.com/user-attachments/assets/7c92664c-a5bd-406f-bf76-827873ccb35b" />

<img width="470" height="270" alt="image" src="https://github.com/user-attachments/assets/a07688ac-f7b3-41f0-96be-714675a551a1" />

<img width="470" height="270" alt="image" src="https://github.com/user-attachments/assets/2c567d0f-4339-40bf-9eef-0866f4c34bb6" />




Trends: 
  
More steps does not necessarily mean that more calories are being burned. The median amount of calories being burned is 2,134- this is a good place to mention that it would be useful to have an age range in the data set as it would help provide deeper insight into trends that the company could leverage to influence its marketing strategy. For example, if we knew that the majority of users were in their early 20’s, we could use that information to run an ad campaign on a popular social media platform (TikTok, Instagram, etc.). 



Key Findings:
 There is considerably less data for more intense activities when compared to the data available for sedentary and light activities. The median time individuals engaged in intense activities ranged from 4-6 minutes; individuals spent 3-17 hours in the other categories of activity that were in the data set (sedentary and light). It would be interesting to further explore this by running a survey or buying more data; what are people mainly using these devices for? Are they trying to track workouts and calories burned, or are they mainly trying to track steps and use the watch to tell the time? Knowing this would directly affect the marketing campaign strategy of the company as it would reveal what individuals are looking to get out of using their products. Another angle to the data that is missing is where users live (are they concentrated in urban areas, or do they live in suburban areas) and the ages of users (this would also reveal usage trends, and directly impact marketing strategy through campaign ideas- e.g. TikTok or Instagram targeting a younger audience, or newspaper ads if users are older). 

One aspect that I believe could make this data even more effective is location: where are the bulk of the users? Do they live in heavily populated urban areas (major cities), or do they live in areas that are not as densely populated (towns and suburbs). I believe that if the company invested in either running a survey or procuring this data, it could make their marketing campaigns much more effective as it would allow them to have insight into the lifestyle trends of their users and that would allow them to tailor their products to fit the lifestyle needs of their customers (both existing and potential). 

Another part of the data that I believe is missing is the length of time of exercise and time of exercise. If there was a field for time (or range of time), you could split the data up to show if the exercise was performed in the morning, afternoon, evening or nighttime. This would be of key interest to the company so they can analyze the trends of their users: having this data would have allowed for an even deeper analysis. 



Recommendations:

Option 1- invest in gathering more data through a survey or buying more data. Would be beneficial to know age, activity types (lifting weights, cross fit, running, etc.), time of activity being performed (morning, afternoon, evening) to more accurately form campaign strategy.

Option 2- if investing in gathering more data is not an option: from the description of the companies products, it may be worthwhile to explore hiring influencers to test the products and post videos on social media platforms showing the products in action. There is quite a big movement on TikTok and Instagram surrounding self-care and fitness so this could give the company the outlet to further expand their reach and position themselves to compete with other players in a similar market.

Option 3- look into the discrepancies in the data mentioned in the summary; the company could potentially invest in revolutionizing how accurately data can be tracked and use that as a marketing ad to either persuade users of other fitness trackers to make the switch to theirs, or persuade individuals thinking about getting a fitness tracker to buy their product over others.


