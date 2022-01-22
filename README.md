# Election Analysis for Denver, Jefferson, and Arapahoe Counties
## Introduction
This audit was conducted in order to gather information about voter turnout in the given tri-county area, as well as to calculate the winner in the election as a whole. This information is useful not only to create a snapshot of voter turnout, but because this code can subsequently be automated and compiled for consecutive election years as a way to gauge voter participation over time in a wide area. 

## Audit Results
- The three counties involved in the audit are as follows: Jefferson (Population 582,910), Denver (Population 705,576), and Arapahoe (Population 656,590). Across all three counties, the total number of votes cast was 369,711. 
- The percentages you will see associated with each county indicates what percent of the total votes came from that county in relation to the others. Denver county by far brought the most votes in this election, which would most likely be due to uneven districting. To be exact, Denver county represents 306,055 votes or 82.8% of the share of votes. Jefferson county represents 38,855 or 10.5% of the share of votes, and Arapahoe county represents 24,801 or 6.7% of the share of votes. 
- The three candidates in the race were Charles Casper Stockham, Diana DeGette, and Raymon Anthony Doane. Diana DeGette won by a landslide, and received 272,892 votes or 73.8% of the total votes. Charles Casper Stockham received 85,213 votes or 23% of the total votes. Raymon Anthony Doane won 11,606 votes or 3.1% of the total votes. 

## Audit Summary and Recommendations for Future
This script does well to inform stakeholders what proportion of the total votes came from the respective counties, but it does little to give insight on participation rates in the election. It would be worth it to include total number of registered or eligible voters in a table that can be referenced after finding the total number of votes per county. This value could then be used to perform a simple division calculation that would yield the voter turnout percentage. 

Another important way in which this script could be improved to allow for broader applications is if the election results themselves were consolidated to include multiple years. From there, the beginning of the script could prompt the user to input a specific year to analyze, and the code that is already written would then be able to iterate over the rows that only correpsond to that year's election data. This would allow stakeholders or those creating visualizations for said stakeholders to be able to run analysis on multiple years of data in relatively quick succession. See Figure 1 below:

![image](https://user-images.githubusercontent.com/92336585/150658083-f7343210-e3d4-4378-ab40-7ed95595d9d4.png)

An _if_ statement could be inserted on line 45 as highlighted. This _if_ statement would come at the beginning of the _for_ loop that begins on line 44 to check that each row corresponds to the user input. 
