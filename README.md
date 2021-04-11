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
###### District Summary![Per_school_analysis_1](https://user-images.githubusercontent.com/79758494/114315899-b244fd80-9ac6-11eb-9e93-a3a2798b2251.PNG)

###### Student Score by School Size![score_by_school_size_1](https://user-images.githubusercontent.com/79758494/114315904-b709b180-9ac6-11eb-9004-038eee860cca.PNG)

###### Student Score by School Type![score_by_school_type_1](https://user-images.githubusercontent.com/79758494/114315908-b8d37500-9ac6-11eb-9c02-f17711890f8c.PNG)

###### Student Score by Average Spending per Student![spending_per_student_1](https://user-images.githubusercontent.com/79758494/114315911-ba04a200-9ac6-11eb-9b29-3799f5394636.PNG)

 
#### Second Analysis and  Results
	To begin the analysis, we first had to import our dependencies, call the file 
	to load, read the school data and student data then store them into a Pandas 
	dataframe, then we cleaned to student names and ensured there were no non-family
	related prefixes or suffixes. 
![Analysis_1](https://user-images.githubusercontent.com/79758494/114316857-1669c080-9acb-11eb-838d-f3af2eaa417d.PNG)

	Numpy was then imported. Loc method was utilized to identify all reading and math
	scores for all ninth graders that attend Thomas High School and replace those test
	scores with NaN. This was executed and can be shown below in the student_data_df 
	dataframe. 
![Analysis_2](https://user-images.githubusercontent.com/79758494/114316858-1669c080-9acb-11eb-902e-1cae23de400e.PNG)

	The data from "student_data_df" and "school_data_df" was merged on "school_name." 
	The resulting dataframe can be seen in the school_data_complete_df below. The
	total count for schools and students were then calculated, along with the total
	budget. The average scores for math and reading were then calculated using the
	"clean_student_data." 
		
	Due to removing all scores for 9th graders at Thomas High School,
	the total number of 9th graders at Thomas High School (THS_9th) was calculated along 
	with the total student count (student_count). The number of 9th graders at Thomas High
	School was then subtracted from the total student count, creating the new student
	count (new_student_count). The resulting new student count is 38,709.
![Analysis_3](https://user-images.githubusercontent.com/79758494/114316860-17025700-9acb-11eb-81ad-02e1ba6bb0f2.PNG)

	Passing rates for the "clean_student_data" was then calculated for both reading 
	and math. Passing percentages for reading and math were then calculated. A 
	dataframe was completed using this data. The dataframe distric_summary_df can be 
	found below. 
![Analysis_4](https://user-images.githubusercontent.com/79758494/114316862-17025700-9acb-11eb-8d62-663bf3f8ceb0.PNG)

	The summary for each school was then calculated and a dataframe was created. 
![Analysis_5](https://user-images.githubusercontent.com/79758494/114316864-17025700-9acb-11eb-9843-1d8ad7cfabc0.PNG)

	The dataframe was then formated. The dataframe, "per_school_summary_df" can be 
	found below. This dataframe shows all the data for each school. 
![Analysis_6](https://user-images.githubusercontent.com/79758494/114316865-17025700-9acb-11eb-8f60-c9f85e47fed7.PNG)

	The above data frame was completed using the data from "school_data_complate_df."
	This data also included all scores from 9th graders at Thomas High School. In order
	to ensure our analysis does not include those scores, the total number of 10th,
	11th, and 12th graders was found, along with the passing percentage of both math
	and reading, and math and reading combined passing score. The percentage was 
	calculated for all three as well. Then, the Average Reading Score, Average Math
	Score, % Passing Math, % Passing Reading, and % Overall Passing were amended with
	this new data in "per_school_summary_df" dataframe.
![Analysis_7](https://user-images.githubusercontent.com/79758494/114316866-17025700-9acb-11eb-86b4-27a3034d7cb9.PNG)

	The amended"Per_school_summary_df" dataframe can be seen below. 
![Analysis_8](https://user-images.githubusercontent.com/79758494/114316867-179aed80-9acb-11eb-855a-8d9aedef310d.PNG)

	The Top 5 and Bottom 5 performing schools were then calculated. Those dataframes
	can be seen below. 
![Analysis_9](https://user-images.githubusercontent.com/79758494/114316868-179aed80-9acb-11eb-91cd-b355256c94b1.PNG)

	Math and Reading scores by grade were then calculated. Series were created for 
	both math and reading and those series were used to create two dataframes: one
	showing math scores per school per grade and the other reading. 
![Analysis_10](https://user-images.githubusercontent.com/79758494/114316869-179aed80-9acb-11eb-8e07-0374038828f5.PNG)
![Analysis_11](https://user-images.githubusercontent.com/79758494/114316870-179aed80-9acb-11eb-97f5-eec396c649db.PNG)
![Analysis_12](https://user-images.githubusercontent.com/79758494/114316871-179aed80-9acb-11eb-816a-55818ba99f66.PNG)

	Scores by school spending was then calculated. This occured by creating bins 
	for the spending ranges and creating group names. Averages were then calculated
	for each column. The data frame "spending_summary_df" was then created and it was
	formatted. 
![Analysis_13](https://user-images.githubusercontent.com/79758494/114316872-179aed80-9acb-11eb-9058-eefed1aa6831.PNG)

	Below is the "spending_sumary_df" Dataframe.
![Analysis_13a](https://user-images.githubusercontent.com/79758494/114316873-18338400-9acb-11eb-9790-84a68a0271f7.PNG)

	By using the same steps as above, the scores by school size were calculated and
	formatted in a new dataframe, "size_summary_df."
![Analysis_14](https://user-images.githubusercontent.com/79758494/114316874-18338400-9acb-11eb-871c-e9356d012904.PNG)

	Below is the "size_summary_df" dataframe. 
![Analysis_14a](https://user-images.githubusercontent.com/79758494/114316875-18338400-9acb-11eb-8d4e-44b735bf5796.PNG)

	Last, the scores by school type dataframe were created. Using the same steps 
	to create the "spending_summary_df" and "siz_summary_df," "type_summary_df" 
	dataframe was created. 
![Analysis_15](https://user-images.githubusercontent.com/79758494/114316876-18338400-9acb-11eb-836f-603793148335.PNG)

	Below is the "type_summary_df" dataframe.
![Analysis_15a](https://user-images.githubusercontent.com/79758494/114316877-18338400-9acb-11eb-8917-7aabc6b37829.PNG)

#### Final Results

    
   -   How is the district summary affected?
		-  During the analysis, after  the "student_data_df" and "school_data_df" were merged, the total count for students was created. That count was 39,170 students. We then calculated a new student score by finding the total number of ninth graders at Thomas High School and subtractin that from our above student count of 39,170. The result was 38,709 students. This is the number moving forward used to calculate new student counts and percentages. 
	    
    -   How is the school summary affected?
	    - Below are the school summaries. The first is the school summary that includes ninth graders at Thomas High School and the second is the school summary after all scores for ninth graders at Thomas High School have been removed.  Specifically looking at the last three columns, which are, respectively, Percent Passed Math, Percent Passed Reading and Overall Percent passed. As shown below, there was a dramatic increase in each of the percentages of passing scores across the board. 

![THS_1](https://user-images.githubusercontent.com/79758494/114320229-9c413800-9ada-11eb-81b9-6dfaca39b90c.PNG)

![THS_2](https://user-images.githubusercontent.com/79758494/114320230-9c413800-9ada-11eb-91de-746c45e9f9c9.PNG)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
	- Compared to other schools, with the 9th grade scores removed, Thomas High School has the second highest overall passing percentage, at 90.6%. If the 9th graders scores had not been removed, Thomas High School would have been in the bottom five performing schools with a 65.1% overall passing. 

- How does replacing the ninth-grade scores affect the following:
	- Math and reading scores by grade: 
		- Replacing the ninth-grades scores only affects the math and reading score by grade by replacing the 9th grade at Thomas High School score with "nan", as seen below in the Math and Reading scores by grade DataFrame.
			![Reading](https://user-images.githubusercontent.com/79758494/114320876-b892a400-9add-11eb-9ef3-a2052fc07c04.PNG)
![Math](https://user-images.githubusercontent.com/79758494/114320877-b892a400-9add-11eb-8948-0dff2f09aa73.PNG)

     -   Scores by school spending
	        - If we were to run the data without updating the data and not including the 9th graders scores at Thomas High School, the result would be the image below:
 ![Spending_`](https://user-images.githubusercontent.com/79758494/114321145-d8769780-9ade-11eb-8aa8-88d46d099ed5.PNG)
 
			 - After removing the 9th graders scores at Thomas High School, the Scores by school spending looks as follows. 
![Spending 2](https://user-images.githubusercontent.com/79758494/114320982-3fe01780-9ade-11eb-90fb-513ba535e795.PNG)

			- Thomas High School has an average student spending of $638.00. They fall into the third row ($630-644). This specific index saw a significant increase in %Passing Math, %Passing Reading, and %Overall Passing, each increasing by 6-7%. 
        -   Scores by school size
	        - The data including the 9th graders at Thomas High School shows the following: ![before_1](https://user-images.githubusercontent.com/79758494/114321372-23dd7580-9ae0-11eb-961d-6ed6709c6550.PNG)
	        
	        - Once we remove the scores for the 9th graders at Thomas High School, the output looks as follows: 
![After_1](https://user-images.githubusercontent.com/79758494/114321373-26d86600-9ae0-11eb-865b-dae1fe0b7501.PNG)

			- Thomas High School has a student population of 1,635 and fall within the "Medium" index. Again, when it comes to the last three columns of data, there was a significant increase in the percentage of students that passed math, reading, and overall. There was a 6% increase throughout each. 

        -   Scores by school type
	        - As with above, the first Database shows all the data including the 9th graders at Thomas High School. The second shows the data after all the scores for the 9th graders at Thomas High School were removed (set as NaN). 

![Before_2](https://user-images.githubusercontent.com/79758494/114321375-293ac000-9ae0-11eb-82ad-fceb80e4ae0a.PNG)

![After_2](https://user-images.githubusercontent.com/79758494/114321380-2c35b080-9ae0-11eb-839f-e184dd6fdd4b.PNG)

- Thomas High School is categorized as a Charter School. As the trend shows, the percentage of passing scores in Math, Reading and overall increased by 3-4%. 

## Summary
It is believed that the 9th grade scores for reading and math were presented with academic dishonestly. If this is the case, that academic dishonestly could have had a large impact on how the school board and superintendent would move forward with funding and programming. This is evidenced by a few things. 

First, before removing all the grades for the 9th Graders at Thomas High School, Thomas High School was ranked as the 8th top performing school. Once the data was amended without the 9th graders scores, Thomas High School ranked as the 2nd top performing school. Second, Scores by school spending went up by 6-7% in the ($630-644) range, where Thomas High School falls. Third, for scores by school type, Thomas High School has a student population of 1,635 and fall within the “Medium” category. There was a 6% increase for each percentage category (% Passing Math, % Passing Reading and % Overall Passing.). Fourth, for scores by school type, the percentage of passing scores in Math, Reading and overall increased by 3-4%.
