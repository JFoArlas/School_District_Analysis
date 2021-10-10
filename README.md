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
  - Thomas High School was ranked second based on their overall passing %, and that did not change after removing their ninth-grade scores
  - The overall passing % did drop just slightly, but not enough to change their ranking

- **Math and reading scores by grade**
  - Before:
  ![image5]()
  
  - After: 
  ![image6]()

- **Scores by school spending**
  - Before:
  ![image7]()
  
  - After: 
  ![image8]()

- **Scores by school size**
  - Before:
  ![image9]()
  
  - After: 
  ![image10]()

- **Scores by school type**
  - Before:
  ![image12]()
  
  - After: 
  ![image13]()

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
