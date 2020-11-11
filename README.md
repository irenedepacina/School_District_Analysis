# School_District_Analysis
Python

Here is the list of deliverables for the analysis of the school district: 

A high-level snapshot of the district's key metrics, presented in a table format
An overview of the key metrics for each school, presented in a table format
Tables presenting each of the following metrics:
Top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score received by students in each grade level at each school
The average reading score received by students in each grade level at each school
School performance based on the budget per student
School performance based on the school size 
School performance based on the type of school

The school district summary will be a high-level snapshot of the district's key metrics:

Total number of students
Total number of schools
Total budget
Average math score
Average reading score
Percentage of students who passed math
Percentage of students who passed reading
Overall passing percentage

To get the percentage of students who passed math and reading, we will write code to:

Determine the passing grade.
Get the number of students who passed math and reading in separate DataFrames.
Calculate the number of students who passed math and reading.
Calculate the percentage of students who passed math and reading.
To get the overall passing percentage, we will write code to:

Get the number of students who passed both math and reading in a DataFrame.
Calculate the number of students who passed both math and reading.
Calculate the percentage of students who passed both math and reading.

Now that we have performed all the calculations needed for the district summary, let's add the following values and columns to a new DataFrame named district_summary_df.

Total number of schools in the column "Total Schools"
Total number of students in the column "Total Students"
Total budget in the column "Total Budget"
Average reading score in the column "Average Reading Score"
Average math score in the column "Average Math Score"
Percentage of students passing reading in the column "% Passing Reading"
Percentage of students passing math in the column "% Passing Math"
Overall passing percentage in the column "% Overall Passing"

The order of the columns in the district_summary_df DataFrame should be as follows:

Total Schools
Total Students
Total Budget
Average Math Score
Average Reading Score
% Passing Math
% Passing Reading
% Overall Passing

This next project requires you to get the following key metrics for each school and place them in a school summary DataFrame. As a reminder, here are the key metrics you're working with: 

School name
School type
Total students
Total school budget
Per student budget
Average math score
Average reading score
% passing math
% passing reading
% overall passing

dig a little deeper into the each school's metadata and get the average math and reading scores for each school. But first, you will need to create DataFrames for each grade level.