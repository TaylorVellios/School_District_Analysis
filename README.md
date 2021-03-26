# School_District_Analysis
Python Pandas

## Overview
An analysis of math and reading scores for highschools across an entire school district.<br>
In this scenario we have been informed of the possibility of academic dishonesty regarding a specific school's scores.<br>
We will be taking a look at the school district as a whole and how the information changes with and without the questionable data.
<br><br>

## Results:
### District Summary
![DistrictSum](https://user-images.githubusercontent.com/14188580/112642476-59603e80-8e11-11eb-8491-1a1fa1cfb5bd.PNG)
<br>

* The District Summary above as well as the School Summary below have been calculated after removing 9th grade scores from Thomas High School.<br>
* Whatever the values were, I used pandas .loc to convert 9th grade data from THS to NaN.
* At our birds-eye view in the District Summary, we can see a trend of greater student aptitude towards Reading compared to Math, as we zoom in we will confirm this.
<br>

### School Summary
![SchoolSum](https://user-images.githubusercontent.com/14188580/112643519-721d2400-8e12-11eb-81e2-f5bc80dbb913.PNG)
<br>

* The School Summary above is being displayed above as a pd.DF copy with formatting for an easier-to-digest visualization. I needed to keep all floats intact for future calculations, but by making a formatted copy I'm able to avoid "chewy" dataframes.
* This Summary contains all of the information that will be used for further data diving.
<br>

![thomas_with_9th](https://user-images.githubusercontent.com/14188580/112650440-62550e00-8e19-11eb-8c18-29d2bd28d9ea.PNG)
<br>
* The jupyter output above shows the average math and reading scores for Thomas High School by grade as well as combined.
* Compared to the rest of the classes at Thomas High School, the 9th grade data does not immediately scream "academic dishonesty". While the math average is the highest among the classes at this high school, the difference is not even 0.1% compared to the next highest class average.
<br>

Compared to the rest of the schools in the district, after removing the 9th grade data; Thomas High School is ranked #2 in terms of overall passing percentage.<br>
![Top5_withNaN](https://user-images.githubusercontent.com/14188580/112651926-de9c2100-8e1a-11eb-8154-a977bc023db5.PNG)<br>
#### Items to Note:
* This data is calculated after converting all Thomas High School 9th Grader scores to NaN.
* Comparing the Average Scores for Thomas High School from the chart above to the highlighted data we saw before NaN conversion, the Average Math Score increased by 0.06% while the Average Reading Score increased by 0.05%.
* Thomas High School's Overall Passing Percentage is 90.63 when removing 9th grade data. When I comment out the conversion to NaN and rerun calculations adjusting for the entire student body at Thomas High School, the new overall passing average can be seen below.
<br>

![ths_overall_withoutNaN](https://user-images.githubusercontent.com/14188580/112654223-2b80f700-8e1d-11eb-8b92-3d0837a622b6.PNG)

<br>
We can conclude that with or without 9th grade data, Thomas High School's standing against the other schools in the district does not change. The difference is neither enough to knock it down a place nor reach first place.
<br>


How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type

Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
