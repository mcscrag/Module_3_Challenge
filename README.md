# Election Analysis

## Processing and Reporting of Election Results

### The goal of this project was to import data directly from a .csv file into python and process it using python scripts to report the results of the election and declare a winner.

## Election-Audit Results

![Election_Results](/Resources/Election_results.png)

* There were 369,711 votes cast in this congressional election.
* Votes broken down by county:
    * Jefferson County - 38,855 votes cast for 10.5% of the total vote.
    * Denver County - 306,055 votes cast for 82.8% of the total vote.
    * Arapahoe County - 24,801 votes cast for 6.7% of the total vote.
* Denver County accounted for the largest voter turnout.
* Votes broken down by candidate:
    * Charles Casper Stockham - received 85,213 votes for 23.0% of the total vote.
    * Diana DeGette - received 272,892 votes for 73.8% of the total vote.
    * Raymon Anthony Doane - received 11,606 votes for 3.1% of the total vote.
* The winner of the election is Diana DeGette who received 272,892 votes for 73.8% of the vote.

## Election-Audit Summary

Applying this python script to other congressional districts in Colorado would present an organizational challenge. Currently the script is using generic file names for the .csv containing the raw election data and writing to a .txt file called *election_analysis*. In order to easily use this script for other congressional districts, I propose two new lines of code. 

First, all .csv files containing raw vote counts need to have a filename that reflects what district they are coming from. For example, the .csv used for this analysis should be renamed to "1st_Congressional_District_Results.csv". 

Next, the following two lines of code need to be added to the script as seen on lines 10 and 11 in the following image. Additionally, the declared variables are put in lines 14 and 16 also seen in the following image.

![Code Change](/Resources/Code_Change_1.png)

Now we can have multiple election results .csv files in the Resources folder and all we need to do is input the filename for these files at the top of the script in line 10 and 11. This will ensure the correct file is being read as well as create a unique .txt file for each congressional district we run the script on. 

