# School_District_Analysis

## Overview of Project
The project studies the academic performance of 15 different schools against various factors.

### Purpose

**Analytical:** The project analyzes the raw data from 15 different schools in the same school district to decipher trends and corelations between the various factors affecting the students' performance in the subjects of math and reading. The analysis also includes cleaning the data to exclude compromised set of of values in order to not skew the results.

**Technical:** The project employs pandas library within python, to perform various functions on DataFrames to see the different visualizations of the same data.

## Results

The analysis is performed on two datasets, referred to as ***old*** and ***new*** hereafter. The 'old' dataset contains compromised data, whereas the new one has all the data deemed unfit for analysis deleted so that accurate resuts can be achieved. Ommiting the untrustworthy data affects all comparisons, please refer to the following to see how it affects different attributes:

#### Effect on District Summary
Old dataset results:
<p align="center">
<img src="/Resources/district_summary_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/district_summary_new.png" width="80%" height="60%">
</p>

**Conclusion:** The results seem to be extremely close to each other (barring how they are formatted, *old* is rounded off to the nearest integer whereas *new* is to 1 decimal place). However, the reason the numbers end up being so close to one another is because the scores omitted only form 1.2% of the total data, and therefore do not have significant affect on the district summary. 

Please note the slight change in the percentage of total students passing math between the old and the new data. There is a difference of 0.89, which is extremely miniscule compared the scale at which these calculations are be done at (order of ten thousands)

| Old | New |
| --- | --- |
| ![Old Math percent results](/Resources/passing_mathp_old.png) | ![Old Math percent results](/Resources/passing_mathp_new.png) |

#### Effect on School Summary

The only values that were changed were the reading and math scores for grade 9 students at Thomas High School, therefore there is no change in the school summary except for the averages of Thomas high school

Old dataset results:
<p align="center">
<img src="/Resources/THS_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/THS_new.png" width="100%" height="100%">
</p>


## Summary
