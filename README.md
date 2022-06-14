# Kickstarting with Excel

## Overview of Project

### Purpose
This analysis was conducted to uncover trends that may be of assistance to Louise, who would like to set up a Kickstarter campaign for a play. To do this, we pulled data of various parameters of Kickstarter campaigns. We then utilized various data analysis tools in Microsoft Excel to investigate inquiries that would be beneficial to Louise planning her campaign. This included: what time of year is the best to launch a successful campaign, and what amount of money is a good goal to set for success.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In order to determine what makes for a successful Kickstarter campaign, one trend we can look to is what time of year is best to launch one. This analysis can help Louise plan which month to launch hers in. We took the data from the Kickstarter dataset to create a pivot table in Excel, and filtered it to display the following information:
- Kickstarter Campaigns specifically under the Theater category.
- Which months they were launched in.
- Whether they were successful, had failed, or were canceled.
- The total number of campaigns per month.

Upon filtering the data in the table, we created a line chart to visually ascertain the relationship between the outcomes and the months the campaigns were launched in:

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106129195/173490708-05fca076-f8e6-4e5a-bf50-a132ab894551.png)

###### The numbers listed vertically to the left represent the number of campaigns, whereas the months listed horizontally represent campaigns launched in that month.

### Analysis of Outcomes Based on Goals

To further assist Louise, we also looked into goal amounts for the campaigns and their outcomes. Determining what is a successful goal range would increase the chances of her campaign succeeding. To determine the relationship between the two, we utilized a powerful formula in Excel to extract information from the Kickstarter data: COUNTIFS. I learned more about how to use the COUNTIFs function [here](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842?ui=en-us&rs=en-us&ad=us). We set up a table with a column displaying ranges of goals from less than 1,000 to 50,000 or more. For those goal ranges, we counted how many were successful, had failed, and were canceled. We also took this information to calculate the percentages of success, failure, and cancelation.

Upon calculating these numbers, we then created a line chart to visually display the information:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106129195/173490725-5f073f13-05b3-4e4c-b140-fd929ec6d030.png)

###### The percentages listed vertically represent the values calculated of successful, failed, and canceled campaigns for Plays. The numbers listed horizontally represent the goal ranges, from less than 1,000 to 50,000 or more.

### Challenges and Difficulties Encountered
A challenge that I encountered while evaluating the dataset, was specifically utilizing Pivot Tables. When looking for specific information to extract from the dataset, it was difficult to determine which variables to present as a filter, column, row, or summation of values. This is an important step for data analysis, as conclusions would potentially be drawn from these tables. To overcome this challenge, I took the time to input different variables in various fields for the pivot table, to better my understanding of where the data gets put in the table.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - Reviewing the chart of Outcomes based on Launch Dates, one conclusion we can draw is that May would be the ideal month to launch a successful Theater campaign. We can see that it has the highest number of successful campaigns. However, June and July would also be suitable months. Conversely, December would be the least ideal month to launch a Theater campaign in. Based on the data, it has the lowest number of successful campaigns compared to the rest of the months.
  - Another conclusion we can draw is that, generally, Theater campaigns have more success than failures, and especially cancelations. Cancelations have a trend of roughly below 10 campaigns each month.

- What can you conclude about the Outcomes based on Goals?
  - Based on the Kickstarter campaign data, we can conclude that if the prospective campaign has a goal of less than 5,000, it has a more favorable chance of succeeding. The chart above shows that there is a slight downward trend at the lower amounts, before dipping down with a steeper slope. While it also shows that there is some success with goals around 35,000 to 44,999, the data pulled shows that there were a total of 9 projects within that goal range. For comparison, the total number of projects with goals of less than 1,000 were 186, and 534 projects with goals between 1,000 and 4,999.

- What are some limitations of this dataset?
  - A limitation discovered while evaluating this dataset, was visibility on Kickstarter's website. While the dataset does provide data for many parameters, it does not contain any information regarding how many times a campaign was clicked open, or "clicks". We would not be able to determine if failed campaigns had any correlation to how many clicks it received, versus whether successful campaigns had more clicks.
  - Another limitation could be the dataset itself. As it is a large dataset, Kickstarter is also a large and well-known website for fundraising campaigns. It is possible that the dataset does not contain information about all campaigns from Kickstarter's somewhat recent history. Therefore, our analysis possibly drew outcomes based off incomplete data.

- What are some other possible tables and/or graphs that we could create?
  - One table and/or graph we could create, to conduct further analysis, would be to look at Campaign Outcomes versus Staff Picks. The analysis could give us, and Louise, information about whether a staff pick increases a campaign's chance of being successful, or if it has any effect at all on the campaign's outcome.
  - Another possible table and/or graph we could create, is looking into Campaign Goals versus Backer Counts. We could potentially investigate whether goal amounts influence someone's decision to back the campaign or not. For example: if the goal is a very high amount (such as more than 45,000), could it possibly deter someone from backing the campaign versus the goal being a low amount (less than 5,000).
