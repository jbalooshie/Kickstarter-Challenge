# Kickstarter-Challenge
Repository for Module 1 Challenge


# Overview of Project
The purpose of this analysis is to provide a detailed breakdown of how different campaigns fared in relation to their launch dates and their funding goals. Specifically, we will provide recommendations on the ideal time to launch a campaign, and how much money the campaign should seek to raise, while still meeting or exceeding its funding goals. We will specifically be focusing on campaigns in the "plays" subcategory on Kickstarter. At the end of this analysis, an individual seeking to launch a Kickstarter campaign to fund a play will have the information they need to maximize their campaign's chances of being funded.


# Analysis and Challenges
Explain how you performed your analysis using images and links to code, as well as any challenges you encountered and how you overcame them. If you had no challenges, describe any possible challenges or difficulties that could be encountered.

## Theater Outcomes by Launch Date

### Analysis

For the first part of our analysis, we looked at the success of campaigns in the "Theater" category, based on the month they were launched in. To do this, we created a pivot table from the raw data. We applied the filters "Parent Category" and "Years", set the columns to show the outcome (successful, failed, or canceled), set the rows to show the date the campaign was created, and the values to the number in each outcome category. Using the filters, we set the table to show only campaigns that had "Theater" as their primary category. We also grouped the dates by month, removing the year and quarter distinctions. Once the pivot table was filtered, we generated the below line graph. 

![Theater Outcomes vs Launch](https://github.com/jbalooshie/Kickstarter-Challenge/blob/main/Theater_Outcomes_vs_Launch.png)

### Challenges

The main challenge here was determining how to set the rows to just show the months. For date categories, the version of excel being used automatically added fields for "Quarters" and "Years". Once these were removed only months were shows.


# Results
Answer the following questions in complete and coherent sentences.
- What are two conclusions you can draw about the Theater Outcomes by Launch Date?
- What can you conclude about the Outcomes based on Goals?
- What are some limitations of this dataset?
- What are some other possible tables and/or graphs that we could create?
