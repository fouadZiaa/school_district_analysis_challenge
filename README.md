# School District Analysis Challenge
PyCitySchools with Pandas

## Challenge Objectives
1. Opening Jupyter Notebook files from local directories using a development environment.
2. Reading an external CSV file into a DataFrame.
3. Formatting a DataFrame column.
4. Determining data types of row values in a DataFrame.
5. Retrieving data from specific columns of a DataFrame.
6. Use of Merge, filter, slice, sort and groupby() in a DataFrame.
7. Use of multiple methods to perform a function on a DataFrame.
8. Performing mathematical calculations on columns of a DataFrame or Series.


## Purpose
A school district asked for a snapshot of several key metrics by each school campus and by the district level.  The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting.  However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspected of dishonesty.  The school board member asked for the data to be removed and analyzed again for a comparison. 

## PythonData Environment
1. Anaconda version 2.1.1
2. Jupyter-Notebook version 6.4.5
3. ipykernal
4. Python version 3.7.7
5. Pandas
6. Numpy


## Results

### How is the district summary affected?
Analysis:

![Pic 1](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/52d52c7e82aacc622b688a8617966bddbb29dae1/Image%201.png)
The testing data of 461 9th graders at Thomas High School was turned into null data, which recalculated the percentages of passing math, passing reading, and the overall passing.  The total count of students did not change as that was run on the count of the student ids, which was not turned into null data. 


When comparing the two charts, removing only 461 test scores had a nominal impact on the almost 40,000 student data set.  The change was less than a 1% difference and the numbers would still round to the same whole number.  

### How is the school summary affected?

In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high.  After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.  

Original Analysis:
![Pic 2](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/1fd6b7199c669390649b332a7da3117e65333081/Screen%20Shot%202022-07-08%20at%201.02.20%20PM.png)

Adjusted Analysis:
![Pic 3](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/8b48952c7c8eaccb90fd812958cd5c420266860e/Screen%20Shot%202022-07-08%20at%201.02.44%20PM.png)

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board. 

Original Analysis:
![Pic 4](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/5478772dd5c081a73eb5dd52204e64c7062b2484/Screen%20Shot%202022-07-08%20at%201.10.40%20PM.png)

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 schools at 8th from the bottom. 

Adjusted Analysis:
![Pic 5](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/6dc432e198f42ff9bf95bb983f017c887f49a6f6/Screen%20Shot%202022-07-08%20at%201.10.59%20PM.png)

## How does replacing the ninth-grade scores affect the following:

### Adjusted Averages using the Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. 
Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts. 

## Adjusted Average Math Scores followed by Adjusted Average Reading Scores

![Pic 6](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/5fb3f09dac19e50bec41c816105086ca995afb4d/Screen%20Shot%202022-07-08%20at%201.16.48%20PM.png)



![Pic 7](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/09eac8c3f5623872246153fe7cf6416d6a3a6148/Screen%20Shot%202022-07-08%20at%201.17.20%20PM.png)

### Scores by school spending

Thomas High School falls in the $630-$644/student spending range.  

Analysis:
![Pic 8](https://github.com/fouadZiaa/school_district_analysis_challenge/blob/5e3fe8248016d0f9b88193b532c3e62b2b17ae3b/Screen%20Shot%202022-07-08%20at%201.31.58%20PM.png)


### Scores by school size
Thomas High School is defined as a medium sized school.  

Analysis:
![Pic 9](https://github.com/


There was very little impact by campus size due to changing the 9th grade scores. 

### Scores by school type

Thomas High School is a charter school type. 

Original Analysis:
![Pic 13](https://github.com/

Adjusted Analysis:
![Pic 14](https://github.com/B

There was very little impact by school type by changing the 9th grade scores. 

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.

