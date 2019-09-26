# dsi_1_danielchang
Analysis of ACT and SAT data

What are the SAT and ACT?
The SAT and ACT are standardized tests taken in high school that are generally used for college admissions decisions and awarding merit-based scholarships. The SAT, or Scholastic Assessment Test, is a standardized test aimed at measuring literacy, numeracy and writing skills. Scores on the SAT range from 400 to 1600, combining test results from two 800-point sections: mathematics, and critical reading and writing. The ACT, originally an abbreviation of American College Testing, is another standardized test divided into four mandatory sections: English, Math, Reading, and Science. The test, as a whole, is graded on a scale of 1-36. 

in the United States, states have experimented between implementing mandatory standardized testing (be it the SAT or ACT), offering free tests, or leaving taking the ACT or SAT up to the discretion of students.

Problem Statement:
In this project, we explore two questions: 1) How does state policy affect SAT/ACT participation scores and composite scores? 2) How are SAT participation and composite scores related?

Contents:
- [2017 Data Import & Cleaning](#Data-Import-and-Cleaning)
- [2018 Data Import and Cleaning](#2018-Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [Descriptive and Inferential Statistics](#Descriptive-and-Inferential-Statistics)
- [Outside Research](#Outside-Research)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

Executive Summary:
The various federal governments in the United States are faced with several challenges in standardizing tests in order to facilitate the massive cross-state exercise of college applications. Several studies have found that the SAT and ACT are good predictors of college performance (see Camara et al @ https://eric.ed.gov/?id=ED446592 for example), and states are keen to set their high school students up for success through good SAT or ACT test scores.

To this end, several states (e.g. DC, Ohio, Colorado) have mandatory tests, but this has received some negative feedback from school administrators, teachers, and students alike as they put a significant amount of pressure on both faculty and students. Furthermore, most of the states with mandatory tests pay for these tests on behalf of their students, and take up a significant portion of their education budget. 

Some states have experimented with offering free, but not mandatory tests. This project aimed to investigate the impact of participation on scores, and how removing the mandatory requirement would affect participation rates. There are psychological theories that suggest that students do better when applying for these tests on their own volition, rather than being forced to take them, but this falls outside the purview of this project and would require further experimentation.

By examining 2017 and 2018 ACT and SAT participation rates and scores, this project finds that participation rates and scores are strongly negatively correlated, and removing the mandatory requirement causes a large dip in participation rates. A caveat for this is that the sample size for states changing their policy mandates are too small to make any reasonable conclusion.

Data Dictionary:
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|The state the test is conducted in| 
|participation|float|ACT/SAT|Percentage of eligible students in a given state who took the test. Values are a percentage, stored as a decimal| 
|act_english|float|ACT|A scaled score between 1 and 36| 
|act_math|float|ACT|A scaled score between 1 and 36| 
|act_reading|float|ACT|A scaled score between 1 and 36| 
|act_science|float|ACT|A scaled score between 1 and 36| 
|act_composite|float|ACT|The ACT composite score is the average of your four area scores, rounded up to the nearest whole number. The score will be between 1 and 36| 
|sat_ebrw|float|ACT|Evidence-Based Reading and Writing - scores are reported on a scale of 200 to 800| 
|sat_math|float|ACT|scores are reported on a scale of 200 to 800| 
|sat_composite|float|ACT|The sum of the Evidence-Based Reading and Writing and Math components, reported on a scale of 400 to 1600| 
