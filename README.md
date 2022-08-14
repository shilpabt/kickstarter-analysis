# Kickstarting with Excel

## Overview of Project

Louise is a play writer and she has a goal of raising $10000 for her upcoming play "FEVER". We have data about current fund raising activities and their results along with other important information. Based on the data Louise wants to understand how to maximize the success of her funding campaigns.

### Purpose
Analyze the data from fundraising activities and gather meaningful insights. With the help of insights suggest Louise about possible approaches which can be used to succeed.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Launch date based chart is as below

![Launch Date Analysis](resources/Theater_Outcomes_vs_Launch.png?raw=true "Outcome based on launch date")
The plan was to create a pivot table and an accompanying chart based on the given data. A new sheet 'Theater Outcomes by Launch Date' was created to present the results for this section. On the main worksheet, I have created a new column 'Years', to get only years from date created convertion, used an YEAR() function. 

The 'Years' column is used as a filter along with 'Parent category' for the pivot table. The rows(x-axis) had 'Date created conversion' and the columns(y-axis) had 'Count of Outcomes', The sum of outcomes. This pivot table was named 'Theatre Outcomes by Launch Date'. Finally, the 'Parent category' was filtered to show data for 'Theater' and for visualization, a line chart was created from the pivot table.

The "Outcomes based on Launch date analysis" reveals following information
* That the month of May have maximum success rate and also that the difference between failed and success is highest in May.
* May to Aug and Oct months have same number of failed campaigns irrespective of number of successes.
* Cancellations can potentially be ignored while analizing the data 

Note that the launch date based analysis sheet provides filters to drill down yearwise data.

### Analysis of Outcomes Based on Goals

![Outcome based on Goals](resources/Outcomes_vs_Goals.png?raw=true "Outcome based on Goals")
A new worksheet is created "Outcomes based on Goals" and the table is created according to the instruction given. I used 'convert to text' to seperate the dollar value ranges 'goal from' and 'Goal to' from the Goal. the COUNTIFS() function was used to populate the number of successful, failed and canceled campaigns. SUM() was used to count the campaigns thats in 'Total Projects'. Percentages were calculated for every outcomes. Finally a line chart, 'Outcomes_Vs_Goals.png', was created for the visualization.

The "Outcomes based on goals" analysis reveals following information
* There were campaigns with fundraising goals between 35,000 - 39,999 and 40,000 - to 44999 to 44999 are as successful as campaigns with fundraising goals of less than 1,000 and between 1,000 - 4,999.
* The data indicates that campaigns with lower fundraising goals have more success, while campaigns with high fundraising goals have lower success.


### Challenges and Difficulties Encountered

* Reason for cancellations were not available to comment on this aspect of data
* The genre of plays might have a role in success or failure and availability of that information would have provided us more insights.
* Instead of writing goal ranges each and every time in couting outcomes, i used convert to text option so that i can divide the goal amount ranges from and goal amout to. Then it was easy to use the column name in first row and drag till the end. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    1. Starting fundraise campaigns in May have higher chances of success
    1. Adding more campaigns in May, Jun, Jul and Aug could potentially increase success rate and potentialy reduce the numbers in Dec as it has highest failure rate.

- What can you conclude about the Outcomes based on Goals?
    1. Larger the goal amount less successful the campaigns were.
    1. In lower value goals less than ($25000), maximum total amount generated out of successful ones is for $1000-$5000 goal amount and this also have success rate of 73%. So maximizing such campaigns will potentially result in reaching target fund early.

- What are some limitations of this dataset?
    1. The genre of plays might have a role in success or failure and availability of that information would have provided us more insights
    1. The data set is not updated one. It is better to have last two years of data to analyse, organize and to incorporate changes.
    1. Reason for the failure/success.

- What are some other possible tables and/or graphs that we could create?
    1. Graph that the success rate of plays by country could reveal more data about how we can spread the plays across contries to maximize success.
    2. Outcomes based on duration of the campaign


