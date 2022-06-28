# Election_Analysis

## Project overview
A Colorado Board of elections employee has provided the following tasks to complete the election audit of a recent local congressional election. 

1. Calculate the total number of votes case.
2. Compile a complete list of candidates who received votes.
3. Calculate the percentage of votes each candidate won.
4. Calculate the total number of votes each candidate won.
5. Determine the winner of the election based on popular vote.
6. Calculate the voter turnout for each county.
7. Calculate the percentage of votes for each county out of the total votes cast.
8. Determine the county with the highest turnout.

## Resources
- Data Source: election_results.csv
- Software:
  - Python version 3.7.6
  - Visual Studio Code version 1.68.1

## Summary
The analysis of the election shows that
- There were 369,711 total votes cast.
- The counties reporting votes were:
  - Jefferson with 10.5% (38,855 votes).
  - Denver with 82.8% (306,055 votes).
  - Arapahoe with 6.7% (24,801 votes).
- Denver county had the largest voter turnout in this election with 82.8% of the votes cast at 306,055 votes.
- The candidates were:
  - Diana DeGette
  - Rayon Anthony Doane
  - Charles Casper Stockham
- The candidate results were:
  - Diana DeGette at 73.8% with 272,892 votes.
  - Rayon Anthony Doane at 3.1% with 11,606 votes.
  - Charles Casper Stockham at 23.0% with 85,213 votes.
- The winner of the election is Diana DeGette with 73.8% of the popular vote (272,892 votes).

## Election-Audit Summary
The script that was written for this election audit process is of such design that it can be used for other election audits as well. By tracking what time votes were cast and manioulating it in a style similar to the counties, we can determine when the majority votes are cast. To do that, we could change the code initializing the county list (county_list = []) into code similar to this (time_entry = []) we could begin to determine during which time frames the most votes are cast. 
Another option would be to track voter turnout for local elections, such a mayor. This could be done using the same script utilized for the candidates in this election. By changing the candidate names, done by updating the source data received, the code would track the winning candidate by popular vote with the same level of detail provided in this audit. Instead of tracking votes by county, the script could be utilized to track by voting precinct (county_votes[county_name] += 1) would become (voting_precinct[precinct_number] += 1).

