# An Analysis of Kickstarter Campaigns.

## Overview of Project

### Purpose
The purpose of this project is to perform analysis with Excel on Kickstarter fundraising campaigns data to uncover trends and help our client to adjust its future campaign projects in the U.S. and Great Britain for the best results.

## Analysis and Challenges

### Analysis of Parent Categrory Outcomes

Since the client is planning a campaign for a play in the U.S. we have taken a look at the Kikckstarter campaigns done in the U.S. Out of the 3038 campaigns done 912 were for the category "theater" which make it the highest in therm of campaign numbers.\
As the following pictures show, "theater" is also the most successful category with 525 successful campaigns lead.

![Parent_Category_Outcomes](https://user-images.githubusercontent.com/68669675/88483437-8b8d6980-cf2d-11ea-9635-2ef9554007d4.png)

![Parent_Category_Outcomes_Theater](https://user-images.githubusercontent.com/68669675/88483433-84665b80-cf2d-11ea-85d7-00be4bf239fc.png)


### Analysis of Subcategory Outcomes

Out of all the Kickstarter campaigns in the U.S., 671 were for plays and over 61% of those campaigns were successful. This makes the plays as the most successful category for Kickstarter campaigns in the U.S.

![Subcategory_Stats_US](https://user-images.githubusercontent.com/68669675/88483646-cd6adf80-cf2e-11ea-89fe-8f6cf3e62d57.png)

![Subcategory_Stats_US_Plays](https://user-images.githubusercontent.com/68669675/88483654-d9ef3800-cf2e-11ea-9a63-bb24b711deaf.png)


### Analysis of Outcomes Based On Launch Date

For this analysis, we are focusing on the campaigns for the category "theater".\
We have produced the PivotChart named "Theater Outcomes Based on Launch Date" from the Kickstarter data. The chart is representing the number of successful, failed and canceled campaigns according the month when the campaign is launched. It is filtered with the parent category "theater" and we are also able to filter by year if we want to focus on a particular period of time.\
We obtained the chart below considering all years for the analysis.

![Theater_vs_LaunchDate_Table](https://user-images.githubusercontent.com/68669675/88729866-70238980-d0fa-11ea-8b3a-fdbffc434327.png)![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/68669675/88729838-6437c780-d0fa-11ea-9c44-39ab2032d6e0.png)


### Analysis of Outcomes Based on Goals

We made an analysis of the outcomes of the Kickstarter campaigns based on their fundraising goals. This time we are focusing on the subcategory "plays".
We had to create a new worksheet containing different fundraising goal amount ranges and we used the Excel function "COUNTIFS()" to populate accordingly the sheet using the following criteria: the outcome of the campaign, the fundraising goal amount and the subcategory "plays".\
We then were able to determine the percentage of successful, failed and canceled campaigns according to the fundraising goal range.\
The following Chart named "Outcomes Based on Goal" was produced.

![Outcomes_vs_Goals_Table](https://user-images.githubusercontent.com/68669675/88729849-69951200-d0fa-11ea-8be6-91e0800a4a59.png)![Outcomes_vs_Goals](https://user-images.githubusercontent.com/68669675/88729822-5d10b980-d0fa-11ea-84a9-49de152b2bbf.png)


### Analysis of Great Britain Musical Outcomes Based on Goals

When focusing our analysis on the subcategory "musical" and the country "Great Britain", we were able to produce the following box plot showing the distribution of the goal and pledged amounts for these campaigns.

![GB_Plays_Distribution](https://user-images.githubusercontent.com/68669675/88491896-4b011080-cf6c-11ea-8586-de3d52c99ece.png)

From these plots, we can see that the mean campaign goal is around £4,000. This is outside of the range of outliers for amount pledged, so the client should probably try to get her musical produced for less than £4,000. Half of the campaign goals are less than £2,000, which is just over the 3rd quartile for amounts pledged, so we would not advise a campaign goal higher than £2,000.


### Challenges and Difficulties Encountered

We did not encounter any particular challenge during the Outcomes vs Launch Date analysis but difficulties could be faced when grouping the launch dates on a monthly basis in the PivotTable.\
The following link gives a good explanation of grouping and ungrouping data in a PivotTable: [Excel documentation](https://support.microsoft.com/en-us/office/group-or-ungroup-data-in-a-pivottable-c9d1ddd0-6580-47d1-82bc-c84a5a340725?ui=en-us&rs=en-us&ad=us). 

When using the COUNTIFS() function, one needs to respect the inputs for that function. I tried to include 2 conditions in 1 criteria using the logical sign "&" as ">=1000 & <4999" but the function only accepts 1 condition per criteria so I had to break the condition into 2 criteria: ">=1000" and "<4999".\
Please find useful information about COUNTIFS() through the following link [Excel documentation](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842?ui=en-us&rs=en-us&ad=us).


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	1. The best period to launch a successful Kickstarter campaign is from May to July.
	2. December is the worst month to launch a campaign since only 50% of the campaigns launched that month have been successful. 

- What can you conclude about the Outcomes based on Goals?\
	The best outcomes are obtained for the fundraising campaigns aiming less than $5,000 and those from $35,000 to $45,000. Above $45,000, most likely the campaign will fail.
 
- What are some limitations of this dataset?\
	Age of data: There is no data after 2017 so we are not working with the most updated set of data to determine the most recent trends.


- What are some other possible tables and/or graphs that we could create?
	1. We could study the Outcomes based on the duration of the campaigns
	2. We could study the Outcomes based on the number of backers.
