# School_District_Analysis
# School District Analysis with Pandas in Jupyter Notebook
## Overview of Project
This project is a Pandas analysis in Jupyter Notebook of a school district of 15 different high schools. The minimum and maximum high school student populations are 427 and 4976, respectively, with a student dataset of 39171 rows by 7 columns and a school dataset of 16 rows by 5 columns. The code, written in Python language, utilizes multiple dataframes to conduct various analyses of the school district. Additionally, due to issues with some of the student names and some of the student scores recorded, this code utilizes various methods to replace values in dataframes.
### Purpose
The purpose of this project is to clean and adjust the student dataset, then provide various analyses of student and school performance across the school district. Some student names were entered with prank suffixes or prefixes, such as "PhD", that needed to be removed in order for the student data to integrate without issues for the school district. Additionally, all of the 9th graders' scores at Thomas High School needed to replaced with NaN due to a discovery of academic dishonesty; the scores were replaced and the analyses were conducted again.
## Results
* Figure 1: District Summary prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 2: District Summary after replacing Thomas High School's 9th grade scores with NaN
  * The only change is the Average Math Score has dropped from 79.0 to 78.9 after replacing Thomas High School's 9th grade scores with NaN
* Figure 3: School Summary prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 4: School Summary after replacing Thomas High School's 9th grade scores with NaN
  * After replacing Thomas High School's 9th grader scores with NaN, in School Summary, Thomas High School's:
    * Average Reading Score increased from 83.4 to 83.9
    * % Passing Math decreased from 93.3 to 93.2
    * % Passing Reading decreased from 97.3 to 97.0
    * % Overall Passing decreased from 90.9 to 90.6
* Figure 5: Top Five Schools prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 6: Top Five Schools after replacing Thomas High School's 9th grade scores with NaN
  * Relative to the other schools, replacing Thomas High School's 9th graders' scores with NaN did not change Thomas High School's position #2 in the top 5 performing schools.
* Figures 7 & 8: Math & Reading Scores prior to replacing Thomas High School's 9th grade scores with NaN
* Figures 8 & 9: Math & Reading Scores after replacing Thomas High School's 9th grade scores with NaN
  * After changing Thomas High School's 9th grade scores with NaN, the only changes to the Math & Reading Scores by Grade are that Thomas High School now reports NaN for their 9th graders' math & reading scores
* Figure 10: Scores by School Spending prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 11: Scores by School Spending after replacing Thomas High School's 9th grade scores with NaN
  * No changes appear in this data
* Figure 12: Scores by School Size prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 13: Scores by School Size after replacing Thomas High School's 9th grade scores with NaN
  * No changes appear in this data
* Figure 14: Scores by School Type prior to replacing Thomas High School's 9th grade scores with NaN
* Figure 15: Scores by School Type after replacing Thomas High Schools's 9th grade scores with NaN
  * No changes appear in this data
## Summary
After replacing Thomas High School's 9th grade scores with NaN, the average reading score for Thomas High School in the school summary increased. Additionally, the district's average math score increased. In order to achieve these new values, the total student count in the district was reduced by subtracting the number of 9th graders at Thomas High School from the total number of students in the district, changing the student count with which we used to calculate new percentages of passing students. Internal changes in Thomas High School's percentages of passing students is due to a change in the number of students used to calculate their results; 9th grade students subtracted from all students at Thomas High School.
