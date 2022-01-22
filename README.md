# Election_Analysis

## Overview of Project

### Purpose

The purpose of this election audit is to evaluate the voter turnout for each county, the percentage of votes from each county out of the total count, and the county with the highest turnout. Finally, we want to find the election results. 

## Analysis

### Election Audit Outcomes

- There were 369,711 votes casted in the congressional election.
- The breakdown of the number of votes and the percentage of total votes for each county is below:
    - Jefferson: 10.5% (38,855)
    - Denver: 82.8% (306,055)
    - Arapahoe: 6.7% (24,801)
- The county with the largest number of votes was Denver.
- The breakdown of the number of votes and the percentage of total votes each candidate received is below:
    - Charles Casper Stockham: 23.0% (85,213)
    - Diana DeGette: 73.8% (272,892)
    - Raymon Anthony Doane: 3.1% (11,606)
- Diana DeGette won the election with 272,892 votes (73.8% of total votes). 

## Election-Audit Summary

### Buisness Proposal 

Every election has candidates and voter turnout. If we were to use this script in other elections, we just have to ensure that the candidate name and the county_name (or any field that we need to figure out the voter turnout from) refers the correct columns respectively. For example, in this case, the candidate name is on column 3 of the file. If the candidate name is on column 5 in the new election, then we must ensure that candidate_name = row[4]. Likewise, if we wish to figure out the voter turnout for a city, and city was column 8 in the new election, then county_name = row[1] should instead read city_name = row[7] and all iterations of the word county within the code should be renamed to city instead. We need to modify the following code to adjust to the new columns.

![Capture](https://user-images.githubusercontent.com/67567087/150656371-47fb93a0-b76d-4215-a4b9-2653fabb047a.PNG)

Also, we may need to be cautious on the invalid votes such as null values in which could be caused by data entry error. For example, there could be a record under candidate name but the county name associated it is missing. In this senario, we would have to eliminate the false record. 

