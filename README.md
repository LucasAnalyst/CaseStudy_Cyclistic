# Cyslistic_bike_share_analysis
---

## About this project

Business Task: Clean, process, and analyze historical trip data over a 12-month period to uncover insights of the divvy trip data( April 2022 - March 2023) to determine differences between casual riders and members. These differences will inform recommendations on a new marketing strategy aimed at recruiting casual riders for annual memberships.

Clear goal: Design marketing strategies aimed at converting casual riders into annual members.

Three questions will guide the future marketing program:
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members

## Preparing the Data: 
---

Use Cyclistic’s historical trip data to analyze and identify trends.

Data Source: [Link here](https://divvy-tripdata.s3.amazonaws.com/index.html)

Data Integrity: The data has been made available by Motivate International Inc. under [this license](https://ride.divvybikes.com/data-license-agreement). This is primary data, collected internally, with no identifying client information.

Data Limitations: To protect the privacy of its users, Cyclistic does not link trip data to individuals. Data can be analyzed only on a single-trip basis. After processing the data, it is clear that there is a large volume of invalid entries, likely caused by canceled transactions and the proper docking of bikes.

From the [Data Source](https://divvy-tripdata.s3.amazonaws.com/index.html), I downloaded the previous 12 months of Cyclistic trip data( from April 2022 to March 2023), and saved it in a local folder; copy and created a sub-folder. 

## Processing Data for analysis
---

### Tool
To process the data from dirty to clean, I'll use Python in VS Code. The previous 12 months of Cyclistic trip data are a large dataset so I think I should use a powerful programming language that offers a number of powerful data processing libraries. Python is a good choice for this task and I'm more familiar with it. After Process and Clean step, I consider using Microsoft Power BI to Analyze and Visualize the data.

### Data Cleaning and Preparation:
Looking for my Python notebook file [here](https://github.com/LucasAnalyst/CaseStudy_Cyclistic/blob/main/Cyclistic_bike_share_clean.ipynb).
- Create a Python environment in VS Code for working with data.
- Use Markdown to document all my work.
- Read and combine 12-month data into one data frame, wrangle it then clean it.
  
There are a few problems we will need to fix:
1. The data type of the start time(started_at) and end time(ended_at) is object.
2. The data can only be aggregated at the ride-level, which is too granular. We will want to add some additional columns of data -- such as day, month, year -- that provide additional opportunities to aggregate the data.
3. We will need to add a calculated field for length of each ride (ride_length) for consistency.
4. Remove/fill "bad" data.

After handling the problems, export the summary file for further analysis.

## Analyze Data Analysis:
---
Key tasks
1. Aggregate your data so it’s useful and accessible.
2. Organize and format your data.
3. Perform calculations.
4. Identify trends and relationships.

I use Power BI for this step. The link of Power BI file is [here](https://drive.google.com/file/d/1h3MlxNFzSJUN589BUT_vuAICKtg16SB0/view?usp=sharing)

![Overview](/Overview.png)

## Share the insights:

After carefully reviewing the data, I found some insights that I can use it to answer the questions Morena asked me. 
I created a presentation file to show my visualizations, including the three top recommendations to convert casual riders into annual members based on my analysis.
Download the presentation file [here](https://github.com/LucasAnalyst/CaseStudy_Cyclistic/blob/main/Cyslistic_bike_share_Presentation.pptx).

##  Recommendations: 
The top Three recommendations are valid strategies to convert casual riders into members and increase customer loyalty for Cyclistic's bike rental service:

1. Use social media and digital ads to target Casual riders with messaging that emphasizes the benefits of membership, such as cost savings and convenience. Especially during weekends and in summer.
2. Consider running marketing campaigns specifically targeting casual riders at the “Streeter Dr & Grand Ave” station. That is a great strategy to remind them of the benefits of membership and encourage them to make a longer-term commitment to the service.
3. Offering discounts or promotions for annual memberships can incentivize casual riders to commit to the service and become loyal customers. This approach can help increase revenue and improve customer retention. Provide incentives for longer biking sessions.

