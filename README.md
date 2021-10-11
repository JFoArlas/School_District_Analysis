# School_District_Analysis

## Overview of the school district analysis
The purpose of the analysis was to use python and Jupyter Notebook to provide the Chief Data Scientist for a city school district with a set of metrics. The data sets included information about students (e.g. grade, school, test scores), and information about the schools those students attend (e.g., type of school, budget, number of students). Once the initial analysis was complete, the school board found that one of the files used to perform this analysis showed evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appeared to have been altered. This required further analysis to exclude the affected scores from the original metrics. This alteration resulted in some changes to the final metrics.

## Results
The math and reading scores for the 9th grade students at Thomas High School were replaced with NaN. This allows us to recalculate Thomas High School's metrics with just the scores from 10th - 12th grade students. Replacing the grades in question with a "0" would not have been proper since that would have brought the average scores for Thomas High School down as if all those students scored 0%.

Replacing the ninth-grade scores this way affected the following metrics:

- **District Summary** - The percentage of students passing math, reading, and the combination of both went down slightly. The average math score also went down slightly, but the average reading score did not change at the district level.
  - Before:
  
  ![image1](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/DistrictSummaryBefore.png)
  
  - After:
  
  ![image2](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/DistrictSummaryAfter.png)

- **School Summary** - The percentage of students passing math, reading, and the combination of both went down slightly. The average math score also went down slightly, but the average reading score actually went up very slightly at the school level. 
  - Before:
  
  ![image3](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/SchoolSummaryBefore.png)
  
  - After:
  
  ![image4](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/SchoolSummaryAfter.png)

- **Thomas High School’s performance relative to the other schools**
  - Thomas High School was ranked second based on their overall passing %, and that did not change after removing their ninth-grade scores.
  - The overall passing % did drop just slightly as seen in the images above, but it was not enough to change their ranking.

- **Math and reading scores by grade**
  - The average scores for math and reading in 10th-12th graders did not change with the removal of the 9th grade scores. 
  - The change is only apparent when you average all of the grades together at the school and district levels.

- **Scores by school spending**
  - Those 461 9th grade students at Thomas High School whose scores were removed were still included in the total number of students at the school. So while the school's scores changed slightly, the school size and per student budget did not change. 
  - The scores for Thomas High School did not change enough to alter the averages for all schools who spend $630-644/student.

![image5](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/Scores%20by%20school%20spending_After.png)
 
- **Scores by school size**
  - Again, because the total number of students was not affected by removing the scores, Thomas High School remained in the "Medium" school size bucket. 
  - The scores for Thomas High School did not change enough to alter the averages for all medium sized schools.

![image6](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/Scores%20by%20school%20size_After.png)

- **Scores by school type**
  - The removal of Thomas High 9th grade student scores does not affect which school type Thomas High School is in.
  - The scores for Thomas High School did not change enough to alter the averages for all Charter school students.

  ![image7](https://github.com/JFoArlas/School_District_Analysis/blob/main/Resources/Images/ScoresBySchoolTypeAfter.png)

## Summary: Replacing reading and math scores with NaNs for the ninth grade students at Thomas High School resulted in the following changes:

1. Thomas High School's Average Math Score went from 83.42 to 83.35
2. Thomas High School's Average Reading Score went from 83.85 to 83.90
3. Thomas High School's % Passing Math went from 93.27 to 93.19
4. Thomas High School's % Passing Reading went from 97.30 to 97.02
