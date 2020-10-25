# Kickstarter Challenge
---------------------------------------------------------------
## Overview of Project
### Purpose
We are trying to help Louise launch her kickstarter campaign. 
She is looking into doing a play kickstarter and we want to know which month of the year has the highest success rate when launched. 
Also, what range of goals had the most successful rate.

## Analysis and Challenges
First, looking at the launch dates in months for the success rates was a challenge for me. 
I had a difficult time figuring out what elements to add to columns, rows, values in the Pivot Table field. 
At the end, it was trial and error that guided me towards the correct table to create the graph. 
![Theater_Outcomes_vs_Launch](https://github.com/female-eugene/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

Second, when going through the outcomes based on goals, I had a tough time with COUNTIFS formula. 
At the end, I came to making this as a bas for the formulas.

=COUNTIFS(Kickstarter!$D:$D, "<1000", Kickstarter!$S:$S, "plays",Kickstarter!$F:$F, "successful") 

However, I was having trouble due to a extra _space in the formula. It kept giving out errors.
Also, I realized I had to lock the rages if I wanted to copy and paste the fomulas. 
At the end, the graph came out to be okay, but it took me a while to change the x-axis and y-axis. 
![Outcomes_vs_Goals](https://github.com/female-eugene/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch](https://github.com/female-eugene/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)
When you look at the graph, it is very clear on the most successful month to launch a campaign. 
May has a high peak. Therefore, I would recommend Louise to launch her Kickstarter in May. 

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://github.com/female-eugene/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)
As you can see on the graph, there are some highs and lows in the successful outcomes. 
It seems like less than 1000 and between 45000 and 49999 seem to have the highest success rates. 

### Challenges and Difficulties Encountered 
However, looking at the dataset, it is difficult to recommend the range of goals for Louise to set a goal. 
30000 to 45000 range seems to have a higher success rate, but the total projects are only 6 and 3. 
That is not enough data points to fully trust the 60% success rate. 
Also, the theater outcomes based on launch dates have some inconsistencies throughout the data. 
When you filter year by year, it is clear that each year success month is different. 
By looking at the agreegated data, May is the highest, but that does not mean it is true for this year. 


#### What are some other possible tables and/or graphs that we could create?
We could filter the most recent years to make the data for Theater Outcomes by Launch Date more relevant. 
I am not sure how to make the Outcomes based on Goals data to be more reliable.
One thing I can think of is using the ranges with more than 36 data points. 
That means Louise won't have data in the higher range of goals. 
