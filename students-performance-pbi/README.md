
# Student Performance Analysis

## Overview

This repository contains an analysis of student performance based on a dataset with 1000 entries. The dataset includes various factors such as gender, race/ethnicity, parental level of education, lunch type, and test preparation course completion. Using Power BI, Power Query, and DAX, several visualizations and insights have been generated to understand the impact of these factors on students' academic performance.

![Students' Performance Dashboard](https://github.com/zinnydigits/students-performance-pbi/blob/main/studentsperformancepbi.PNG)


## Dataset Description

The dataset consists of 1000 entries with the following columns:

- **gender**: Male or Female
- **race/ethnicity**: Group A, B, C, D, or E
- **parental level of education (PLOE)**: Various levels of education
- **lunch**: Standard or free/reduced
- **test preparation course (TPC)**: Completed or none
- **math score**: Scores in mathematics
- **writing score**: Scores in writing
- **reading score**: Scores in reading

## Analysis Tools and Techniques

### Tools Used

- **Power BI**
- **Power Query**
- **DAX**

### Analysis and Visualizations

1. **Average Score Calculation**: 
   A new column, `average score`, was added to the dataset, representing the average of math, writing, and reading scores.

2. **DAX Code Snippet**:
   ```dax
   Bins = 
   VAR BinSize = 10
   VAR MaxValue = 100
   VAR CurrentValue = [average score]

   RETURN 
   IF(
       CurrentValue >= MaxValue,
       MaxValue - BinSize,
       FLOOR(CurrentValue, BinSize)
   )
   ```
   This DAX formula creates bins needed for histogram for the average score.

3. **Visualizations**:
   - **Card Visualizations**: Displayed minimum, maximum, average scores and total students.
   - **Gauges**: Showed overall students' average scores for math, writing, and reading.
   - **Histogram**: Created using a DAX formula on a clustered column chart to display the distribution of average scores, which appears to follow a normal distribution.
   - **Combo Chart**: Combined line and column charts to display the number of students and their average scores based on parental level of education.
   - **Scatter Plot**: Showed the relationship between reading and writing scores, revealing a positive linear correlation.
   - **Bar Chart**: Compared students with standard lunch and those who completed the test preparation course to those who did not, showing that the former group generally performed better.

## Key Findings

- The students are 52% females and 48% males.
- Best Average score: 100, Lowest average score: 9 and Overall average: 67.77.
- There is a high correlation between writing and reading score.
- Group C is the most populated ethnic group while group E has the best academic performance.
- Students who had standard lunch and completed their test preparation course perform better than students with free/reduced lunch and did not complete their test preparation course.

The students' performance [Power BI Dashboard](https://github.com/zinnydigits/students-performance-pbi/blob/main/studentsperformance.pbix) and [students performance dataset](https://github.com/zinnydigits/students-performance-pbi/blob/main/StudentsPerformance.csv) are all uploaded on this repository.
