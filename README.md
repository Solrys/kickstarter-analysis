# kickstarter-analysis
Performing analysis on kickstarter data to uncover trends

## Overview Of Project

### Background:
The Purpose of this analysis is to provide Louise with data on how various campaigns fared in relation to their launch date and funding goals. Louise, a playwright, expressed an interest in this specific data after her play _Fever_ came close to its fundraising goal in a short amount of time. Looking to the outcomes of other Kickstarters will shed light on variables that contributed to success so that Louise may be able to potentially mirror this success for her future campaigns.

### Strategy and Metrics:
I will be using Excel to organize, sort, and analyze crowdfunding data. I will be creating focused datasets and visualize campaign outcomes based on their launch dates and their funding goals. I will be taking a closer look into Kickstarter campaigns that are in the Theatre Category, as well as the Play Subcategory to provide Louis with more concentrated data based on her field.The data will be divided into the following two categories:
1)Outcomes Based on Launch Dates (for theatre)
2)Outcomes Based on Goals (for plays)

### Results:
I will analyze the data for trends and provide results and conclusions. I will disclose the limitations of this data to offer a more balanced view on my findings. This analysis will inform Louise on optimal launch dates and goals. These insights may be used to help prepare Louise for successful upcoming kickstarters in her field. 


## Analysis and Challenges

### Analysis For Outcomes Based On Launch Date:
Analysis For Outcomes Based On Launch Date:
For the first part of this analysis I will examine the outcomes based on the launch date. In order to clearly visualize this, I  isolated the year each kickstarter was launched. This was achieved by creating a new column (“Years”) from the original Kickstarter spreadsheet. I used the YEAR() function to extract the year from the “Date Created Conversion” column. In order to focus the data, a Pivot table was created with a filter for the “years” and the “Parent category”.  The parent category filter was set to “Theatre”
In order to visualize this data the following line chart was created. 

![Theater_Outcomes_vs_Launch](kickstarter-analysis/Recources/Theater_Outcomes_vs_Launch.png
g).

### Challenges For Outcomes Based On Launch Date:
While this data is insightful it only reflects the outcome patterns for the Parent Category “Theatre”. A similar method of deriving outcomes based on a launch date for the subcategory “Plays” may reinforce our derived data or prove a new insight. We also have don’t have enough data to derive why the summer months perform better than the winter months. 

### Analysis For Outcomes based on Goals:
In this next part I have compiled data pertaining to the outcomes of kickstarters based on their goal amount. The Goals are divided into 12 categories of ascending bracketed goal amounts. We then measured the success, failure, and cancellations for each of those rows. This information was populated by using a COUNTIFS () formula pulling data from the original Kickstarter sheet into a new table. Once The amount of goals for each category of outcomes was retrieved, I was able to derive the total number of projects for each row using the SUM() function. After that step was complete and I calculated the total number of projects, I was able to determine a percentage for each outcome by dividing the results by the total number of projects in the same same bracket (=B2/BE). After populating the columns of percentage of successful, failed, and canceled outcomes for each row, I created a line chart titled "Outcomes Based on Goals” to visualize the relationship between the goal amount and relative outcomes. In order to visualize this data I created the following line chat:

![Outcomes_vs_Goals](kickstarter-analysis/Recources/Outcomes_vs_Goals.png).

### Challenges For Outcomes Based on goals:
The main challenge working on this dataset was that the amount of total projects for each bracket of goals was not consistent. 


## Results:

### Results  For Outcomes Based On Launch Date:
Looking at the chart we can learn two main points. 
1) May was the most successful month for Theatre kickstarters. 
2) December was the least successful month for Theatre kickstarters. 
At a closer look the surrounding summer months faired well while the surrounding winter months performed poorly. 
In addition, while we only looked at the parent category Theatre, examining other facets of this data could help strengthen an argument for a predictable trend. It may also be useful to compare this data in relationship to the amount of kickstarters started through the months to see how many campaigns were launched in the winter months in comparison to the summer months. 

### Results For Outcomes based on Goals:
The data from this chart illustrates that the campaigns with the lowest goals were most successful. Because none of the campaigns were cancelled, the percentage of failed campaigns perfectly negates the successful ones to form an opposing correlation on the graph. This information is consistent as the percentage of goals drops until we reach the bracket of $25,000 to $29,999. 
The reason for inconsistency after that is a result of a much smaller total projects for the ascending goal brackets. Creating a minimum requirement of 20 total projects for each goal bracket (in this case $0-$29,999) will allow for a more balanced view in how goal correlates to outcome and will remove possible outliers from this data.

### Conclusion:
Based on my Analysis it is clear that May is the best month to launch a theatre kickstarter (111 successful outcomes, 52 failed) while December shows the least promise (37 successful outcomes, 35 failed). 
In addition having a smaller goal for play kickstarter is preferable. Goals under $1000 had the highest percentage of successful outcomes (75.81%)
Although there are more total projects for the lower goal brackets, we have shown that the difference is not statistically significant until we research goals with less than 20 total projects per goal bracket and therefor a trend may still be determined.  
