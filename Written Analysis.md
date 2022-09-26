# election-analysis

## Overview of Election Audit: 
### Explain the purpose of this election audit analysis.

The purpose of this analysis was to take the results of the election, drill down into the data, and create a comprehensive overview of the findings such as: 
- the total number of votes cast in the election
- who was running in the election
- which counties were involved
- which county and candidate was attributed with the largest amount/percentage of votes.


## Election-Audit Results: 
Using a bulleted list, address the following election outcomes. Use images or examples of your code as support where necessary.

### How many votes were cast in this congressional election?
- 369,711 Total Votes were cast in this congressional election.

### Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

For every county that was included in the election, a for loop retrieved the county vote count by setting that variable to "ballots" (ballots = county_votes[county_name]) and calculated the percentage of votes for the county by dividing the total votes by "ballots" and multiplying it by 100 (ballots_percentage = float(ballots) / float (total_votes) * 100).

Then we printed the county results to the terminal:
- Jefferson county was responsible for 10.5% of the total votes or (38,855) votes.
- Denver county was responsible for 82.8% of the total votes or (306,055) votes.
- Arapahoe county was responsible for 6.7% of the total votes or (24,801) votes.

### Which county had the largest number of votes?
- Denver county had the largest number of votes.

### Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

In a similar manner that we collected counties, a for loop retrieved the vote count and percentage.

Then we printed each candidate's voter count and percentage to the terminal using an F-String:

candidate_results = (
            f"{candidate_name}: {vote_percentage:.1f}% ({votes:,})\n")

- Charles Casper Stockham received 23.0% of the total votes or (85,213) votes.
- Diana DeGette received 73.8% of the total votes or (272,892) votes.
- Raymon Anthony Doane received 3.1% of the total votes or (11,606) votes.

### Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
- Diana DeGette won the election with 272,892 votes, which is 73.8% of the total votes.


## Election-Audit Summary: 
### In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections.

This script could have been used to show the best places to campaign based on each candidates platform and what percentages of the population by gender or age votes for each kind of candidate.
