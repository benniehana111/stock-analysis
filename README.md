# Kickstarting with Excel

## Overview of Project

### Purpose

This project documents the outcomes of funding campaigns for theatre productions, showing how their funding success varies based on the month in which campaigns are launched and the size of their funding goals. It is based on a dataset of Kickstarter campaigns from 2009 to 2017 which included 1,369 theatre productions, of which 1,047 were plays. This dataset included the name and description for each Kickstarter campaign, the funding goal, funds pledged, launch date of the funding campaign, and several additional variables not used in this project.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To analyze the relationship between funding campaign success and the month in which they were launched, this project includes a pivot table displaying the number of campaigns which succeeded, failed, or were canceled based on the month in which the campaigns were launched. This table is presented in a line graph titled “Theater Outcomes Based on Launch Date” which displays the number of funding campaigns on the y-axis and the launch month of the campaigns on the x-axis. 

Theater_Outcomes_by_Launch_Date.png

This graph allows the viewer to visually compare the number of successful, failed, and canceled campaigns in each month of the year. The highest success rate for funding campaigns occurs in the month of May when approximately 2/3 of all campaigns (111 out of 166) succeed; this is also the peak month for launching campaigns. The number of successful campaigns continually declines from June through December (to a low of 37), then rebounds to an intermediate range (56 to 71) in January through April.

The lowest success rates occur in the month of December when only about 1/2 (37 out of 75) of all campaigns achieve their funding goal. The number of failed campaigns per month is more stable, ranging from a low of 31 in November to a high of 52 in May. Canceled campaigns are relatively uncommon; only 37 cancellations occurred out of 1,369 funding campaigns.

### Analysis of Outcomes Based on Goals

To analyze the relationship between funding campaign success and the size of funding goals, this project includes a pivot table displaying the number of campaigns which succeeded, failed, or were canceled based across twelve funding levels ranging from less than $1,000 to greater than $50,000. This table is presented in a line graph titled “Outcomes Based on Goal” which displays the percentage of funding campaigns on the y-axis and the size of their funding goals along the x-axis. 

Outcomes_Based_on_Goal.png

This graph allows the viewer to visually compare the percentages of successful, failed, and canceled campaigns based on the size of their funding goals. The highest funding success rates occur in campaigns seeking less than $5,000. The proportion of failed campaigns rises steeply as the funding goal increases, surpassing the number of successful campaigns at funding goals above $20k. 

The apparent high rate of success for campaigns in the $35-45k range is based on a very small number of observations (9 plays; less than 1% of the dataset) and could simply be an outlier. If the funding ranges in the table were broadened (e.g., <$5k, $5-15k, $15-25k, $25k> then this apparent spike in success rates would disappear. However, there is a possibility that this result is driven by a cohort of well-run theatre companies that operate at that scale, but we could only support such a conclusion with additional data that identified those specific companies. Funding targets exceeding $45,000 are most likely to fail; only two out of seventeen campaigns in this range achieved their funding goal.

### Challenges and Difficulties Encountered

This analysis lacks predictive value due to the limited data available; cursory statistics on funding campaign success indicate that success is maximized by starting a Kickstarter campaign in May and seeking less than $5,000 in funding. It provides no other insights for how to improve chances for successful fundraising. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  May is the best month for launching Kickstarter funding campaigns for theater productions; this is when the most campaigns are launched and when the probability for success is the greatest. December is the worst month; when the fewest campaigns are launched and when the probability for success is lowest.

- What can you conclude about the Outcomes based on Goals?

  Funding goals of less than $5,000 are relatively easy to achieve; funding success becomes progressively more difficult as goals increase beyond $5,000. More data on the fundraising organizations is needed to identify what factors drive success of theater Kickstarter campaigns for larger amounts.

- What are some limitations of this dataset?

  The dataset provides few details on the internal attributes of each funding campaign; the only variables are the number of financial backers and whether a production was a “staff pick” or “spotlight.” There is no information on the individuals and organizations associated with each funding campaign, so we can’t tell if there are people with track records of success or failure. 

- What are some other possible tables and/or graphs that we could create?

  We should merge the two data threads analyzed here to examine if the size of funding goals varies by month and if there is any correlation between fundraising success, timing, and the size of fundraising goals. A first cut at this analysis would come include four line graphs similar to “Theater Outcomes by Launch Date,” with each graph corresponding to a fundraising level (e.g., <$5k, $5-15k, $15-25k, $50k>).

  We should map funding success rates against other variables provided in the data set – country, staff pick, spotlight, # of backers, and average donation size – to see if there are any correlations. These graphs would mirror the form of the “Outcomes Based on Goal” graph, replacing the x-axis value (funding goal) with other variables (or combinations of variables).
