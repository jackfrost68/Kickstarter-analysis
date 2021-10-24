## An Analysis of Kickstarter Campaigns 


# Overview of Project
As an up and coming playwright, Louis sought my help before she started a campaign for her play, “Fever”.  In order to develop insights that will help her make better informed decisions, I analyzed past crowdfunding data using Excel. 


# Analysis and Challenges

To analyze the dataset, I leveraged the present data to create new columns such as Average Donations and Percentage Funded. Furthermore, I implemented tools such as sort, filter and pivot tables. 

![This is an image](https://github.com/jackfrost68/Kickstarter-analysis/blob/7edd40c204fa336c1018b9e85d6f51bd40ce77f1/Screen%20Shot%202021-10-24%20at%202.51.33%20PM.png)


Additionally, I used conditional formatting to easily visualize the percentage funded per play.In order to help visualize results from my pivot tables, I inserted pivot charts. Lastly, to determine if there were any outliers, I plotted a box and whiskers chart. 

![This is an image](https://github.com/jackfrost68/Kickstarter-analysis/blob/7edd40c204fa336c1018b9e85d6f51bd40ce77f1/Box%20and%20whisker%20plot.png)



*Challenges* 

1. DIV/0 error
When calculating the Percentage Funded or the Percentage Canceled, the denominator had 0 hence causing the DIV/0 error. In order to fix this, I used the IFERROR formula that would print a 0 or 0% instead of the error. 

2. UNIX timestamps
The original deataset’s dates were stored in the UNIX format. To solve this, I converted these timestamps to a month/day/year format that is easily readable and understandable. I did this by dividing the numbers by 60 (seconds), 60 (minutes) and lastly 24 (hours). 


# Results 

*Based on Launch Date* 

1. Most theatre-based campaigns are likely to succeed in July. 
2. For most theatre-based campaigns, they are more likely to fail in January. 

![This is an image](https://github.com/jackfrost68/Kickstarter-analysis/blob/7edd40c204fa336c1018b9e85d6f51bd40ce77f1/Outcomes%20Based%20on%20Launch%20Date.png)


*Based on Goals*

According to past data, campaigns with a goal of $25,000 to $29,999 have an 80% of failure. However, if Louise set her goal less than $1,000 or between $35000 - $39,999, she has a 76% and 67% chance of succeeding respectively. 

![This is an image](https://github.com/jackfrost68/Kickstarter-analysis/blob/c6d6be28412df2944b1351a7a9e10bd46e5c633c/Outcomes_vs_Goals.png)

# Limitations of dataset 
There is missing data for canceled theatre campaigns between the months of March and May 

# Recommendations 
1. Additional chart analyzing outcomes based on staff picks i.e. whether having more staff picking Louise’s play would make it more likely to succeed. 
2. A chart analyzing outcomes based on country in order to help Louise figure out where to run her campaign and optimize her donations. 
 
