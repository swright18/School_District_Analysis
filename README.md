# School District Analysis
### Purpose
---
This analysis of data uses Python Pandas to analyze city's school district data around funding and test scores for 9th-12th graders in the areas of reading and math. This project will help the school board and superintendent to make strategic decisions regarding future school budgets at the school and district level. 

### Overview
---
In this analysis, data from 15 schools and 39,170 students in the school district was aggregated to find trends and school performance. After completing the analysis, the school board determined that there is evidence of academic dishonesty in the students_complete.csv file for the reading and math grades for 9th Graders at Thomas High School. The school board is wanting a new analysis completed, removing the reading and math scores for 9th graders at Thomas High School. 

### Resources
---
- Data sources: 
	- schools_complete.csv
	- students_complete.csv
- Software:
	- JupyterNotebook using Python
	- Numpy
	- Pandas software library

## Results


#### First Analysis  Results
###### District Summary
![Per_school_analysis_1](https://user-images.githubusercontent.com/79758494/114315899-b244fd80-9ac6-11eb-9e93-a3a2798b2251.PNG)
###### Student Score by School Size
![score_by_school_size_1](https://user-images.githubusercontent.com/79758494/114315904-b709b180-9ac6-11eb-9004-038eee860cca.PNG)
###### Student Score by School Type
![score_by_school_type_1](https://user-images.githubusercontent.com/79758494/114315908-b8d37500-9ac6-11eb-9c02-f17711890f8c.PNG)
###### Student Score by Average Spending per Student
![spending_per_student_1](https://user-images.githubusercontent.com/79758494/114315911-ba04a200-9ac6-11eb-9b29-3799f5394636.PNG)
 
#### Second Analysis and  Results
	To begin the analysis, we first had to import our dependencies, call the file 
	to load, read the school data and student data then store them into a Pandas 
	dataframe, then we cleaned to student names and ensured there were no non-family
	related prefixes or suffixes. 
![Analysis_1](https://user-images.githubusercontent.com/79758494/114316857-1669c080-9acb-11eb-838d-f3af2eaa417d.PNG)
![Analysis_2](https://user-images.githubusercontent.com/79758494/114316858-1669c080-9acb-11eb-902e-1cae23de400e.PNG)
![Analysis_3](https://user-images.githubusercontent.com/79758494/114316860-17025700-9acb-11eb-81ad-02e1ba6bb0f2.PNG)
![Analysis_4](https://user-images.githubusercontent.com/79758494/114316862-17025700-9acb-11eb-8d62-663bf3f8ceb0.PNG)
![Analysis_5](https://user-images.githubusercontent.com/79758494/114316864-17025700-9acb-11eb-9843-1d8ad7cfabc0.PNG)
![Analysis_6](https://user-images.githubusercontent.com/79758494/114316865-17025700-9acb-11eb-8f60-c9f85e47fed7.PNG)
![Analysis_7](https://user-images.githubusercontent.com/79758494/114316866-17025700-9acb-11eb-86b4-27a3034d7cb9.PNG)
![Analysis_8](https://user-images.githubusercontent.com/79758494/114316867-179aed80-9acb-11eb-855a-8d9aedef310d.PNG)
![Analysis_9](https://user-images.githubusercontent.com/79758494/114316868-179aed80-9acb-11eb-91cd-b355256c94b1.PNG)
![Analysis_10](https://user-images.githubusercontent.com/79758494/114316869-179aed80-9acb-11eb-8e07-0374038828f5.PNG)
![Analysis_11](https://user-images.githubusercontent.com/79758494/114316870-179aed80-9acb-11eb-97f5-eec396c649db.PNG)
![Analysis_12](https://user-images.githubusercontent.com/79758494/114316871-179aed80-9acb-11eb-816a-55818ba99f66.PNG)
![Analysis_13](https://user-images.githubusercontent.com/79758494/114316872-179aed80-9acb-11eb-9058-eefed1aa6831.PNG)
![Analysis_13a](https://user-images.githubusercontent.com/79758494/114316873-18338400-9acb-11eb-9790-84a68a0271f7.PNG)
![Analysis_14](https://user-images.githubusercontent.com/79758494/114316874-18338400-9acb-11eb-871c-e9356d012904.PNG)
![Analysis_14a](https://user-images.githubusercontent.com/79758494/114316875-18338400-9acb-11eb-8d4e-44b735bf5796.PNG)
![Analysis_15](https://user-images.githubusercontent.com/79758494/114316876-18338400-9acb-11eb-836f-603793148335.PNG)
![Analysis_15a](https://user-images.githubusercontent.com/79758494/114316877-18338400-9acb-11eb-8917-7aabc6b37829.PNG)
#### Final Results
 Using bulleted lists and images of DataFrames as support, address the following questions.
    
    -   How is the district summary affected?
    -   How is the school summary affected?
    -   How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    -   How does replacing the ninth-grade scores affect the following:
        -   Math and reading scores by grade
        -   Scores by school spending
        -   Scores by school size
        -   Scores by school type
## Summary
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
