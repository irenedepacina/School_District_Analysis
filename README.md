# School District Analysis

## Overview of the School District Analysis 
This analysis showcases a high-level snapshot of a school district's key metrics, presented in a table format. The following values and columns were added to a new DataFrame:

- Total number of schools in the column "Total Schools"
- Total number of students in the column "Total Students"
- Total budget in the column "Total Budget"
- Average reading score in the column "Average Reading Score"
- Average math score in the column "Average Math Score"
- Percentage of students passing reading in the column "% Passing Reading"
- Percentage of students passing math in the column "% Passing Math"
- Overall passing percentage in the column "% Overall Passing"

An overview of the key metrics for each school, presented in a table format. The tables presented each of the following metrics:
- The summary of each distrct
- The summary of each school
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

### Purpose
The purpose of this analysis was to recalculate the values and columns in the original DataFrame. The original data regarding Thomas High School (THS) ninth graders was inaccurate and unreliable. The ninth grades' math and reading scores from Thomas High School was replaced and denoted as a missing value. The math, reading, and overall passing percentages had to be recalculated based on the new total student count. The THS ninth graders had been subtracted from the total student count. By repeating the school district analysis, I was able to compare the new results with the old results. 

## Results 
- How is the district summary affected?
    - By replacing the Thomas High School ninth graders, the average math score, % passing math, % passing reading, and % overall passing decreased. The ninth graders had high values and by setting the ninth graders as null, the percentages declined.
    - ![old](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/district_summary_old.png)
    - ![new](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/district_summary_new.png)
- How is the school summary affected?
    - For Thomas High School, the school summary highlights that percentages increased substantially after the removal of the THS ninth graders.
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_summary_old.png)
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_summary_new.png)
- How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
    - Replacing the ninth graders' math and reading scores does affect the Thomas High School's performance relative to the other schools. According to the school rankings, Thomas High School now sits at 2nd place when the ninth grade scores are replaced in the dataset. In the original data, Thomas High School was not in the top 5 schools. 
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/top_5_old.png)
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/top_5_new.png)
    - Below are the bottom 5 performing schools based on overall passing rate. The results remain unchanged.
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/bottom_5_old.png)
    - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/bottom_5_new.png)
- How does replacing the ninth-grade scores affect the following - included are before and after images of the tables:
    - Math and reading scores by grade
        - The ninth grade and Thomas High School cell is denoted with a NaN. That is the only difference. However, the math and reading scores for grades 10-12 are unchanged because they are dependent on variables that are not attributed to the ninth grade math and reading scores.
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/math_scores_by_grade_new.png)
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/reading_scores_by_grade_new.png)
    - Scores by school spending
        - There is no change. The scores by school spending are unchanged because the total number of students and budgets are the same. Therefore, the percentages are also the same.
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_spending_old.png)
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_spending_new.png)
    - Scores by school size
        - There is no change. The school size and the updated metrics have remained the same.
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/size_summary_old.png)
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/size_summary_new.png)
    - Scores by school type
        - There is no change. The school type and the updated metrics have remained the same.
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_type_old.png)
        - ![](https://github.com/irenedepacina/School_District_Analysis/blob/main/Resources/school_type_new.png)

## Summary
Four major changes to the school district analysis after the reading and the math scores had been replaced:
1. The percentage of passing math, reading and overall was a major change. By replacing the ninth graders as null, it was required to calculcate the total ninth grades students from the Thomas High School student count by subtract that value from the total student count across all the schools. The new student count changed the percentages mentioned above because the denominator changed causing a decrease in the district summary.
2. The district summary saw a decrease in the percentages. The metrics Average Math Score, % Passing Math, % Passing Reading, % Overall Passing decreased by 0.1%, 0.2%, 0.1%, and 0.3% respectively.
3. The math and reading scores by grade tables output NaN in the ninth grade and Thomas High School cell.
4. The school summary saw a increase in most percentages. The metrics % Passing Math, % Passing Reading, % Overall Passing increased by 26.27%, 27.36%, and 25.55% respectively. The reason for the major change is due to the fact the grades of 10th to 12th graders from THS are included in the percentages. A potential explanation for the substantial increase is due to the fact the denominator has decreased and the low grades of the ninth graders are taken out, causing the percentages to increase. 
