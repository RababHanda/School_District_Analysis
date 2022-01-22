# School_District_Analysis

## Overview of Project
The project studies the academic performance of 15 different schools against various factors.

### Purpose

**Analytical:** The project analyzes the raw data from 15 different schools in the same school district to decipher trends and corelations between the various factors affecting the students' performance in the subjects of math and reading. The analysis also includes cleaning the data to exclude compromised set of of values in order to not skew the results.

**Technical:** The project employs pandas library within python, to perform various functions on DataFrames to see the different visualizations of the same data.

## Results

The analysis is performed on two datasets, referred to as ***old*** and ***new*** hereafter. The 'old' dataset contains compromised data, whereas the new one has all the data deemed unfit for analysis deleted so that accurate resuts can be achieved. Ommiting the untrustworthy data affects all comparisons, please refer to the following to see how it affects different attributes:

#### Effects on District Summary
Old dataset results:
<p align="center">
<img src="/Resources/district_summary_old.png" width="60%" height="40%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/district_summary_new.png" width="60%" height="40%">
</p>

**Conclusion:** The results seem to be extremely close to each other (barring how they are formatted, *old* is rounded off to the nearest integer whereas *new* is to 1 decimal place). However, the reason the numbers end up being so close to one another is because the scores omitted only form 1.2% of the total data, and therefore do not have significant affect on the district summary. 

Please note the slight change in the percentage of total students passing math between the old and the new data. There is a difference of 0.89, which is extremely miniscule compared the scale at which these calculations are be done at (order of ten thousands)


| Old | New |
| --- | --- |
| ![Old Math percent results](/Resources/passing_math%_old.png) | ![Old Math percent results](/Resources/passing_math%_new.png) |


| Old | New |
| --- | --- |
| <p align="center">
<img src="/Resources/passing_math%_old" width="100%" height="100%">
</p> | <p align="center">
<img src="/Resources/passing_math%_old" width="100%" height="100%">
</p> |



- The county of **Denver** had the largest turnout of voters
- Out of a total of 3 candidates, Charles Casper won *23%* of the total, Diana DeGette *73.8%* and Raymon Anthony Doane *3.1%*:

- As a clear indication from the graph above, **Diana DeGette** won the election by a landslide, bagging **272,892** votes in total (*73.8%*)

## Summary

The script used for this audit is universal as it determines all values and factors while reading the data, therefore it can be easily used for analysing any such results. In this report we only determine the turnout per county and the votes per candidate, however this script can be modified to achieve the following results as well:

1. **Votes cast per candidate from each county:** this can help determine how the population of a couty reacts to the candidate's manifestos, the winner from each county - as that might be different from the overall winner, etc. The most populated counties will have the power to sway the results to their favour, provided the turnout is proportional to the population.

    - To do so we will need to declare a new dictionary (which will have nested dictionaries in it). This new dictionary will have the following structure
    ```python
    votes_candidate_county = {
        'county1' : {'candidate1': votes1, 'candidate2': votes2, 'candidate3': votes3}
        'county2' : {'candidate1': votes2_1, 'candidate2': votes2_2, 'candidate3': votes2_3}
        'county3' : {'candidate1': votes3_1, 'candidate2': votes3_2, 'candidate3': votes3_3}
    }
    ```
    - Then, once the candidate_options and the county_options lists have been populated, we can add a for loop (line 74 for reference) to go through each county, get the votes for every candidate in that county. The following piece of code will do the work:
    ```python
    for candidate in candidate options
    ```

2. 

### Modification Suggestions

| Objective | Modificaion |
| --- | --- |
| Votes cast per candidate from each county | List all new or modified files |
| git diff | Show file differences that haven't been staged |