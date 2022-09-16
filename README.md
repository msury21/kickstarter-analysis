# Kickstarting with Excel

## Overview of Project

After Louise's campaign quickly neared it's goal, she wanted to know about other campaigns with such information as their goals and amounts pledged, when they were started and how long they lasted, their location, and their type. 

### Purpose

The purpose of this analysis is to study the Kickstarter data and compare the results of various campaigns in relation to their launch dates and to their fundraiser goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To analyze the outcomes based on the launch date, I created a Pivot Table that showed the results of theater fundraising campaigns based on the month they were launched in, and then created a line graph from that table

![Theater_Outcomes_vs_Launch](kickstarter-analysis/Resources/Theater_Outcomes_vs_Launch.png)

From this chart it can be seen that theater campaigns have more successes than failures no matter the month a campaign is launched, though the margin varies. Theater campaigns launched in May have the greatest margin of success to failure and those launched in December have the least. Very few theater campaigns are canceled, but those launched in Jaunary have the most cancellations at seven.

### Analysis of Outcomes Based on Goals

To analyze the outcomes based on the goals of the campaigns for plays, I created a table which had as the independent variable the goal a campaign set for itself in ranges from Less Than 1000 to 50000 or More. The dependent variables were the number of of successful, failed, and cancelled campaigns, the total amount of campaigns, and the percentage of those campaigns that were successes, failures, or cancellations. To find number of plays that were successfully funded for each range of goals, I used the COUNTIFS function to count how many successful plays were within each such range. I similarly used the COUNTIFS function for the amount of failed and cancelled plays. I then used the SUM function to find the amount of total campaigns for each range of goals, and then found the percentage of successes, failures, and cancellations for each range. Then, I created a line graph which would display the percent of plays that were successfully funded, failures, and cancelled compared against the range of goals.

![Outcomes_vs_Goals](kickstarter-analysis/Resources/Outcomes_vs_Goals.png)

From this graph, it can be seen that, except from 15000 to 34999 and 45000 and more, there is a larger amount of successes than failures. There are also zero play campaigns that were cancelled. The ranges of goals that has the highest amount of success is those that had a goal of less than 1000 at 76% and 1000 to 4999 at 73%. The success rate continues to decrease, being outweighed by the failures once the goals start to hit the 20000 to 24999 mark. Additionally, in the 45000 to 49999 range there are absolutely no successful fundraising campaigns for plays (though there is only 1 play within that range). Interestingly enough, the second two highest ranges of goals are 35000 to 39999 and 40000 to 44999, both at 67%.

### Challenges and Difficulties Encountered

One challenge I encountered was figuring out how to configure the Pivot Table for analyzing the outcome of theater campaigns based on the launch date to only show the month as the rows, as opposed to the year of launch. Other than that, it was a little bit of a struggle to figure out how to use the COUNTIFS function, but once I did some reading on it, I was able to figure it out.

## Results

From the graph for Theater Outcomes Based on Launch Date, I can conclude that May is the best time to launch a fundraising campaign for a theater project and December is the worst time. From the graph for Outcomes Based on Goals, I can conclude that it is best to have the goal for plays' fundraising campaigns below $5000. A limitation of this dataset is that it does not show outside influence, such as social media or being showcased on the news. Some other possible graphs that could be created are those that compare amount of the goal to the length of the campaign, which would show how much time people estimate is needed to raise a certain amount, the average donation by type of campaign, to see if certain types of campaigns draw wealthier people, and whether a campaign being a staff pick or spotlighted influenced its results.