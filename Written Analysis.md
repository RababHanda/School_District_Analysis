# School_District_Analysis

## Overview of Project
The project studies the academic performance of 15 different schools against various factors.

### Purpose

**Analytical:** The project analyzes the raw data from 15 different schools in the same school district to decipher trends and corelations between the various factors affecting the students' performance in the subjects of math and reading. The analysis also includes cleaning the data to exclude compromised set of of values in order to not skew the results.

**Technical:** The project employs pandas library within python, to perform various functions on DataFrames to see the different visualizations of the same data.

## Results

The analysis is performed on two datasets, referred to as ***old*** and ***new*** hereafter. The 'old' dataset contains compromised data, whereas the new one has all the data deemed unfit for analysis deleted so that accurate resuts can be achieved. Ommiting the untrustworthy data affects all comparisons, please refer to the following to see how it affects different attributes:

#### 1. Effect on District Summary
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


#### 2. Effect on School Summary

The only values that were changed were the reading and math scores for grade 9 students at Thomas High School, therefore there is no change in the school summary except for the averages of Thomas high school

Old dataset results:
<p align="center">
<img src="/Resources/THS_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/THS_new.png" width="80%" height="60%">
</p>

**Conclusion:** as can be seen in the percentages above, the difference between old and new summaries isn't much, and that is again due to the fact that the changed dataset comprises 1 grade out of 4 for which the averages are being calculated. Even with the difference, the overall results would remain unchanged should the numbers be rounded off to the nearest integer

|  | % Passing Math | % Passing Reading | % Overall Passing |
| --- | --- | --- |--- |
| Difference | -0.9 | -0.29 | -0.31 |


#### 3. Performance Relative to Other Schools

As mentioned in the conclusion of the 2nd point, there is <1% of difference between the old and new results. Even when the rankings are compared, Thomas High School still ranks at the 2nd place according to the overall passing percentage. The school's performance remains unaffected relative to the others in the district.


#### 4. Effect on Scores by Grade

Because the scores for all 9th graders at Thomas High School were changed to NaN, the new scores arranged by grade reflect that change. Other than that there are no changes in the scores for other grades at Thomas High School or any other schools. 

|  | Old | New | 
| --- | --- | --- |
| Math Scores | ![Old Math percent results](/Resources/bygrade_math_old.png) | ![Old Math percent results](/Resources/bygrade_math_new.png) | 
| Reading Scores | ![Old Math percent results](/Resources/bygrade_reading_old.png) | ![Old Math percent results](/Resources/bygrade_reading_new.png) | 


#### 5. Effect on Scores by School Spending

Old dataset results:
<p align="center">
<img src="/Resources/spending_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/spending_new.png" width="80%" height="60%">
</p>

**Conclusion:** The total budget for Thomas school is $1,043,130 with per student being $638, thus falling in the second highest category of spending, there is one other school in that category. Therefore, despite the change in scores of 416 pupils, the change isn't reflected at the higher level because that forms a small percentage of the total values used to calculate these numbers


#### 6. Effect on Scores by School Size

Old dataset results:
<p align="center">
<img src="/Resources/size_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/size_new.png" width="80%" height="60%">
</p>

**Conclusion:** There are number of students in Thomas High School, 416 of whom the scores were replaced for. 

#### 7. Effect on Scores by School Type

Old dataset results:
<p align="center">
<img src="/Resources/type_old.png" width="80%" height="60%">
</p>
New dataset results:
<p align="center">
<img src="/Resources/type_new.png" width="80%" height="60%">
</p>

**Conclusion:** There are number of students in Thomas High School, 416 of whom the scores were repla

## Summary


