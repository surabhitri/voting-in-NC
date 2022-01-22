# voting-in-NC
### Voting in NC (2020 General Elections)
#### Introduction
The North Carolina State Board of Elections (NCSBE) is the agency charged with the administration of the elections process and campaign finance disclosure and compliance. Among other things, they provide voter registration and turnout data online (https://www.ncsbe.gov/index.html, https://www.ncsbe.gov/results-data). Using the NC voter files for the general elections in November 2020, you will attempt to identify/estimate how different groups voted in the 2020 elections, at least out of those who registered. Here’s an interesting read on turnout rates for NC in 2016: https://democracync.org/wp-content/uploads/2017/05/WhoVoted2016.pdf (you might consider creating a similar graphic to the one on page 4).

Data
The data for this part of the project can be found on Sakai. The file voter_stats_20201103.txt contains information about the aggregate counts of registered voters by the demographic variables; the data dictionary can be found in the file DataDictionaryForVoterStats.txt. The file history_stats_20201103.txt contains information about the aggregate counts of voters who actually voted by the demographic variables.

You will only work with a subset of thoe overall data. Take a random sample of 25 counties out of all the counties in both datasets. You should indicate the counties you sampled in your final report. You will need to merge the two files voter_stats_20201103.txt and history_stats_20201103.txt by the common variables for the counties you care about. Take a look at the set of join functions in the dplyr package in R (https://www.rdocumentation.org/packages/dplyr/versions/0.7.8/topics/join) or the merge function in base R. I recommend the functions in dplyr. You may choose to merge the datasets before or after selecting the samples you want, but be careful if you decide to do the latter.

Questions of interest
Your job is to use a hierarchical model to answer the following questions of interest.

How did different demographic subgroups vote in the 2020 general elections? For example, how did the turnout for males compare to the turnout for females after controlling for other potential predictors?
Did the overall probability or odds of voting differ by county in 2020? Which counties differ the most from other counties?
How did the turnout rates differ between females and males for the different party affiliations?
How did the turnout rates differ between age groups for the different party affiliations?
