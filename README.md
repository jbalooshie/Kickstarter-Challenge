# Kickstarter-Challenge
Repository for Module 1 Challenge


# Overview of Project
The purpose of this analysis is to provide a detailed breakdown of how different campaigns fared in relation to their launch dates and their funding goals. Specifically, we will provide recommendations on the ideal time to launch a campaign, and how much money the campaign should seek to raise, while still meeting or exceeding its funding goals. We will specifically be focusing on campaigns in the "plays" subcategory on Kickstarter. At the end of this analysis, an individual seeking to launch a Kickstarter campaign to fund a play will have the information they need to maximize their campaign's chances of being funded.


# Analysis and Challenges
This section explains how the analysis was performed, and details any challenges encountered. It is divided between the main variables we were looking at, how the launch date for the campaign affected the campaign outcome, and how the goal amount affected the campaign outcome. 

## Theater Outcomes by Launch Date

### Analysis

For the first part of our analysis, we looked at the success of campaigns in the "Theater" category, based on the month they were launched in. To do this, we created a pivot table from the raw data. We applied the filters "Parent Category" and "Years", set the columns to show the outcome (successful, failed, or canceled), set the rows to show the date the campaign was created, and the values to the number in each outcome category. Using the filters, we set the table to show only campaigns that had "Theater" as their primary category. We also grouped the dates by month, removing the year and quarter distinctions. Once the pivot table was filtered, we generated the below line graph. 

![Theater Outcomes vs Launch](https://github.com/jbalooshie/Kickstarter-Challenge/blob/main/Theater_Outcomes_vs_Launch.png)

### Challenges

The main challenge here was determining how to set the rows to just show the months. For date categories, the version of excel being used automatically added fields for "Quarters" and "Years". Once these were removed only months were shows.

## Outcomes Based on Goals

### Analysis 

For the second part of our analysis, we looked at the percentage of successful campaigns in the "Plays" subcategory, based on their fundraising goals. First, we created 12 different dollar amount ranges between $0-50,000 (<$1000, $1000 - $4999, $5,000 - $9,999, etc.). We then used the COUNTIF function to count the number of successful, failed, and canceled campaigns within each range. Here is the formula used to determine the number of successful campaigns in the $1000 - $4999 band:

'=COUNTIFS(Kickstarter!$D:$D,">=1000", Kickstarter!$D:$D,"<=4999",Kickstarter!$F:$F,"Successful",Kickstarter!$P:$P,"Plays")'

This was done for reach fundraising range and outcome. We then totaled the number of campaigns in each range. From the total, we then calculated the percentage of each outcome within each fundraising range. Using those percentages, we created the following line chart:

![Outcomes vs Goals](https://github.com/jbalooshie/Kickstarter-Challenge/blob/main/Outcomes_vs_Goals.png)

### Challenges

For this section, the main challenge was a typo in one of the ranges. Instead of creating two separate ranges: $30000 - $34999 and $35000 - $39999, one range was created combining the two: $30000 - $39999. This resulted in the line chart not matching the example provided. Once this range was fixed and the formulas updated, the chart matched the example.



# Results
Answer the following questions in complete and coherent sentences.
- What are two conclusions you can draw about the Theater Outcomes by Launch Date?
- What can you conclude about the Outcomes based on Goals?
- What are some limitations of this dataset?
- What are some other possible tables and/or graphs that we could create?
