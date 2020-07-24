# Project 1: SAT & ACT Analysis


## Executive Summary
1. Problem statement

>College Board changed the SAT in 2016 so now we need to see how well it is being received by the states, and which state(s) may need to receive extra attention by College Board. To do this I am using the available 2017-2018 data for SAT/ACT participation and scores. Using the participation data I will narrow down which states to focus on, and hopefully some ideas on how to increase participation in those states.

2. Description of data:

	Data size:
	 >Final Data shape is (51x17)
	
	Data source:
	 >Source for [SAT data](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/)
	
	 >Source for [ACT data](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows)
	
	Data Dictionary:

|Feature|Type|Dataset|Description|
|---|---|---|---|
***state***|object|N/A|Names of states in the US, includes the Washington D.C.
***part_sat_2018***|float64|2018 SAT Averages|The percentage of students who took the SAT in 2018, ordered by state.
***read_sat_2018***|int64|2018 SAT Averages|Average SAT Evidence-Based Reading and Writing score of students in 2018, ordered by state.
***math_sat_2018***|int64|2018 SAT Averages|Average SAT Math score of students in 2018, ordered by state.
***totalsat_2018***|int64|2018 SAT Averages|Average SAT total score of students in 2018, ordered by state.
***part_act_2018***|float64|2018 ACT Averages|The percentage of students who took the ACT in 2018, ordered by state.
***comp_2018***|float64|2018 ACT Averages|Average ACT composite score of students in 2018, ordered by state.
***part_sat_2017***|float64|2017 SAT Averages|The percentage of students who took the SAT in 2017, ordered by state.
***read_sat_2017***|int64|2017 SAT Averages|Average SAT Evidence-Based Reading and Writing score of students in 2017, ordered by state.
***math_sat_2017***|int64|2017 SAT Averages|Average SAT Math score of students in 2017, ordered by state.
***totalsat_2017***|int64|2017 SAT Averages|Average SAT total score of students in 2017, ordered by state.
***part_act_2017***|float64|2017 ACT Averages|The percentage of students who took the ACT in 2017, ordered by state.
***eng_act_2017***|float64|2017 ACT Averages|Average ACT English score of students in 2017, ordered by state.
***math_act_2017***|float64|2017 ACT Averages|Average ACT Math score of students in 2017, ordered by state.
***read_act_2017***|float64|2017 ACT Averages|Average ACT Reading score of students in 2017, ordered by state.
***science_act_2017***|float64|2017 ACT Averages|Average ACT Science score of students in 2017, ordered by state.
***comp_2017***|float64|2017 ACT Averages|Average ACT composite score of students in 2017, ordered by state.

3. Findings:

>One way to increase participation in a state is to of course to increase mandatory testing. This seems like a short-term win here though. Colorado and Illinois certainly show how a mandatory SAT test can swing participation from 10% to 100%, but there is no reason this can't happen in a few years for ACT. States like Tennessee allow their school districts to make the decision regarding whether to require SAT or ACT testing. So both the regional location and the internal small localities are avenues College board should work.
 
3. Recommendations:

>Recommendations:
-Increase state contracts, but this tends to be zero-sum
-Reach out more to local governments and school districts
-Keep funding SAT School days. This has been a popular program.
-Adapt to the new STEM focus. Math sections have a greater effect on total score vs ACT.
-Perhaps highlight portions showcasing ‘algorithmic/programmatic thinking’ etc.

>Pros for the states:
-Focus on school districts and local government. Midwest and
South often leave testing decisions up to school districts.
--ESSA gives states more ability to allow counties/districts
to make assessment decisions.
-Using SAT instead of state-created assessments is cheaper and
tests competencies better. This also makes compliance with
ESSA simpler.
-Ohio allows SAT scores above a certain level to be another path
to a high school diploma. Also makes compliance with ESSA
simpler.
-Continuity for the large number of students who take PSAT.

>Further data I could use:
-More granular data at the local level (counties, parishes, school boards etc.)
-PSAT data. How often does a student take the PSAT and then go on to take the SAT?