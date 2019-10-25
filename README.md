# School_District_Analysis

## Project Overview
Here is a list of deliverables for the analysis of the school district:
- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
  - Top 5 and bottom 5 performing schools, based on the overall passing rate
  - The average math score received by students in each grade level at each school
  - The average reading score received by students in each grade level at each school
  - School performance based on the budget per student
  - School performance based on the school size
  - School performance based on the type of school
  
## Resources
- Data Source: schools_complete.csv, students_complete.csv 
- Software: Anaconda 4.7.12, Jupyter Notebook, Pandas, PythonData environment using Python 3.6

## Summary
By the end of this module, we will be able to:
- Open Jupyter Notebook files from local directories using a development environment.
- Read an external CSV file into a DataFrame.
- Format a DataFrame column.
- Determine data types of row values in a DataFrame
- Retrieve data from specific columns of a DataFrame
- Merge, filter, slice, and sort a DataFrame.
- Apply the groupby() function to a DataFrame.
- Use multiple methods to perform a function on a DataFrame.
- Perform mathematical calculations on columns of a DataFrame or Series.

## Challenge Overview
Maria and her supervisor have discovered that the score averages for ninth graders from one high school are incorrect. Maria has asked to remove the math and reading scores for that high school, but without removing those ninth-grade students from the analysis.

- Filter DataFrames using logical operators.
- Replace the incorrect values with NaN.
- Explain how your PyCity Schools analysis changes after you handle the incorrect data.

## Challenge Summary
The analysis of the schools, after removing the reading and math scores, show that:

### District Summary <br/>
| Total Schools  | Total Students | Total Budget   | Av Math Score | Av Reading Score| % Passing Math | % Passing Read | % Overall Pass| 
| -------------- |:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|--------------:|
| 15             | 39,170         | $24,649,428.00 | 79             | 82             | 75             | 86             | 80            |
| 15             | 39,170         | $24,649,428.00 | 79             | 82             | 74             | 85             | 79            |
| 15             | 39,170         | $24,649,428.00 | 78.93          | 81.86          | 73.88          | 84.65          | 79.27         |

The district summary is affected by replacing the reading and math scores for ninth graders at Thomas High School with NaN as shown in the table above. The first row of data is from PyCitySchools.ipynb, before we replaced the incorrect values with NaN. The second row of data is from PyCitySchools_Challenge.ipynb. This row shows a 1% decrease in the % Passing Math, % Passing Reading, and % Overall Passing columns after replacing the incorrect values with NaN. It was odd that the Average Math and Reading Score was not affected. In the third row of data I allowed the scores to be rounded to the nearest hundredth, after we replaced the incorrect value with NaN. Allowing this shows that the Average Math and Reading Scores were affected. The Total Schools, Total Students, and Total Budget columns were not affected.

Thomas High School is the only school affected in the school summary.

### Thomas High School <br/>
| School Type    | Total Students | Total School Budget| Per Student Budget| Av Math Score| Av Reading Score | % Passing Read | % Overall Pass| 
| -------------- |:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|--------------:|
| 15             | 39,170         | $24,649,428.00 | 79             | 82             | 75             | 86             | 80            |
| 15             | 39,170         | $24,649,428.00 | 79             | 82             | 74             | 85             | 79            |
| 15             | 39,170         | $24,649,428.00 | 78.93          | 81.86          | 73.88          | 84.65          | 79.27         |

Removing the ninth graders' math and reading scores only affects Thomas High School by showing NaN 
- Removing the ninth-grade scores affect the Math and Reading Scores by:
  - Grade
  - Scores by School Spending
  - Scores by School Size
  - Scores by School Type


