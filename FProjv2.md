ECOB2000 Final Project
================
Patrick Sinclair

#### Introduction

Statistical research on education outcomes commonly hones in test scores
and graduation rates, outcomes used by the government and academia alike
as broad metrics for institutional success. The research provides
insights for policy directions to manage issues including outcome gaps
due to race and ethnicity differences (Reardon et al. 2016),
socioeconomic status differences (Owens 2010) and overall student
achievement levels (Grosskopf et al. 2015). There is a subsection of the
literature that focuses on the impact and efficiency of educational
resources. Predominantly this research has sought to find correlation
between resource availability or allocation and educational attainment.

This paper uses the U.S. Department of Education 2017-18 Civil Rights
Data Collection, National Center for Education Statistics Common Core of
Data 2017-18 Lunch Program Eligibility Survey and the U.s. Department of
Education EDFacts Data Set 2017-18 Chronic Absenteeism Table (DG 814) to
test for a correlation between school resources and the rate of chronic
absenteeism in schools. Chronic absenteeism is defined as missing 15 or
more days of school (U.S. Department of Education 2019). Chronic
absenteeism can have negative impacts on educational achievements across
all levels of education (Balfanz 2016).

Utilizing a composite data set comprised of variables from the three
original data sets, the paper estimates Chronic Absentee rates in
schools with a variety of resource and student variables. The estimates
demonstrated that non-financial resource variables are statistically
significant at the 95% level while financial resource variables do not
produced correlations with any notable statistical significance.
Further, student variables showed significance in their correlations
with chronic absenteeism. The results imply that resource allocation
within many schools is not optimal and the resources that are serving
students are not impacting rates of chronic absenteeism.

#### Literature Review

The statistical literature on education outcomes has generally focused
on assessment scores and graduation rates as functions of cost and
socioeconomic inputs. The use of these as dependent variables are useful
in that they give a clear picture of how students perform and an
indication of how education institutions are operating from an ‘end
goal’ perspective. Some studies have focused on analyzing standardized
test results in order to compare outcomes across the United States
(Houtenville and Smith Conway 2008; Reardon et al. 2016). The use of
standardized test scores as the output metric enables educational
outcomes to be assessed across states and school districts. This is an
important point as there is autonomy in the curriculum even as low as
the district level (Reardon et al. 2016). Accordingly, normalized
student level gains in mathematics and reading is one of the most common
measures of school district output (Grosskopf et al. 2015).

Despite the convenience of standardized test scores as outputs they can
present challenges to the researcher. The State and District focus on
maximizing student performance on standardized tests can detract from
less measurable educational outcomes. In practice, it “may cause
teachers and schools to divert resources away from nontested topics and
skills” and in an analytical sense “potentially biases estimates of
teacher quality by ignoring teachers’ effects on students’ character
skills and related behaviors.” (Gershenson 2016, p. 127). Further,
standardized test scores provide a narrow measure of student outcomes
(Greene et al. 2007). Other studies have examined smaller State and
District level data, allowing researchers to make comparisons at the
school level, minimizing the difference in assessment standards. Many
resource focused studies have used data at the state and district levels
to analyze impacts on educational attainment resulting from financing
(Cellini et al. 2011), resource quality (Greene et al. 2007), resource
allocation (Iatarola and Rubenstein 2007). Across much of the
literature, school resources have been found to be have less of an
impact on student test scores or graduation rate than student
demographic and background factors.

The discussion amongst the literature on school resources and student
educational attainment must begin at the decision of which resources to
choose as variables. There is some consensus that utilizing finance and
expenditure is a valid proxy for available resources. Hedges et
al. performed a meta-analysis of studies between 1993 and 2014 that
included per pupil expenditure (PPE) as a correlate of student
achievement (Hedges et al. 2016). The authors of that study raise an
important point in regard to studies of school resources as correlates
of student outcomes: different studies focus on different input
variables and use different outcome measures. That said, PPE is a common
proxy for per student resource allocation. Hedges and his co-authors
find that there is “a nonstatistical relationship between PPE and
student achievement” (Hedges et al. 2016). This finding echoes the
findings of Hanushek (Hanushek 1989) who came to similar conclusions in
1986 and 1997 (Grosskopf 2013).

The key implication of the nonstatistical relationship between PPE and
student outcomes is the impact of school-external factors. That is to
say, the background of the student has a bearing on that student’s
educational outcome that is uninfluenced by school spending. In her 2010
study of 11,097 middle and high school students, Ann Owens utilizes
racial and socioeconomic composition variables to determine the impact
on high school graduation rates and college matriculation rates among
students in low-similarity and high-similarity cohorts, controlled
against PPE (Owens 2010). The results of Owens’ study demonstrate that
students from a low socioeconomic neighborhood tend to have their odds
of educational attainment lowered when in a cohort with a high
proportion of class mates from a high socioeconomic background. She also
found “that racial composition may proxy school climate or structural
characteristics that affect educational attainment” (Owens 2010). An
issue with the racial composition finding may be that the author only
used proportions of white and black residents, other ethnicities were
not included in the models.

Where Owens uses racial composition to proxy structural characteristics,
David Branham uses a percentage of free and reduced price lunch eligible
students as a proxy for the proportion of the cohort living in poverty.
The study examines the effects of physical school resources, such as the
use of temporary buildings and state of structural repair, on student
attendance and drop-out rates (Branham 2004). Branham includes student
and teacher effects as controls. His findings suggest that schools with
poor physical resources - in a state of disrepair or heavily reliant on
temporary structures - are less likely to have students attend school.
However, the coefficients Branham calculated from his models are
significant to 0.01 and 0.05 in one-tailed tests.

Teacher based variables present in the literature include
student-teacher ratio, not to be conflated for class size. Greene
explains that the student-teacher ratio “…assesses the availability of
human resources for instruction…” (Greene et al 2007). Teacher
experience and teacher quality are also variables that could have an
influence on various student outcomes that are not adequately addressed
in an expenditure variable such as PPE. Houtenville and Smith Conway
include the percentage of teachers with Masters and Doctoral degrees as
one of five school characteristics. The percentage of teachers with
advanced degrees can be viewed as a proxy for “instructional quality”
(Greene et al. 2007).

In a study linking teacher quality and student attendance, Gershenson
weights teacher experience more heavily in the calculations for teacher
effects. “Attendance is an objectively measurable behavior” that is
linked with character skills (Gershenson 2019). Absenteeism is an
opposite behavior that can have a negative impact on a student’s
educational outcome. Based on the literature regarding the effect of
school resources on student outcome, the rest of this paper will outline
and analyze school effects, students effects and resources as correlates
of rates of chronic absenteeism.

#### Data

The data used is a dataset comprised of variables from the U.S.
Department of Education 2017-18 Civil Rights Data Collection (CRDC),
National Center for Education Statistics Common Core of Data 2017-18
Lunch Program Eligibility Survey (CCD) and the U.s. Department of
Education EDFacts Data Set 2017-18 Chronic Absenteeism Table (DG 814)
(EDFacts). The datasets were able to be linked together due to a common
identifier, “COMBOKEY”, that is a composite number of a Local Education
Agency (LEA) number and a School number (SCH). Issues with these
datasets are they do not give individual student level data, and they
are self-reported, leaving the collected data vulnerable to reporting
mistakes.

The CRDC is the main dataset used to complete the dataset. It is for the
School Year 2017-18 and comprises data from 17,637 LEAs and 97,632
schools. The mix of schools includes Elementary, Middle, High, Magnet,
Charter, Alternative, Special Education and Justice Facility schools.
The EDFacts data is a supplemental file containing, among other
elements, information on Chronic Absenteeism for 92,438 schools. Lastly,
the CCD dataset contains 494,746 observations: Free lunch eligible,
reduced price lunch eligible, missing data and NA values for
approximately 123,687 schools.

The CRDC dataset is disaggregated by race, gender, English learner
status and disability status. It comprises of multiple data groups. To
create the data for the models, the COMBOKEY variable was used to match
the following data groups: School Characteristics, School Expenditure,
Enrollment, Dual Enrollment, Gifted and Talented, Transfers, Retention
and School Support with Chronic Absenteeism and Free and Reduced Price
Lunch Data. The common observations reduced the original number of
observations from 97,632 to 89204 common observations.

Justice Facility schools (162) were removed from the data, leaving
89,042 observations. Then the data was cleaned for any reserve codes.
They were predominantly codes indicating that schools had not reported
complete data and had their observations force certified by the
Department of Education or that the school did not submit any
information in time and completed an action plan to complete information
for the next survey (52), leaving 88,990 observations. There were issues
with the number of Absent Students and Free and Reduced Price Lunch
Eligible students exceeding Total Enrolled Students. These schools were
removed. Finally, schools with less that 15 students, 1 full time
equivalent teacher or spent zero dollars on Teacher Salary, Support
Staff Salary, Personnel Expenditure or Non-Personnel Expenditure were
also removed. The final dataset was left with 71,667 schools.

Some variables were added to the dataset, to create totals for
enrollment, proportions for Enrolled Minorities, Limited English
Proficient students and Free and Reduced Price Lunch eligible students,
per pupil expenditure, inexperience teacher to teacher ratio, teacher
plus support staff salary to personnel expenditure ratio, average
teacher salary and the proportion of chronically absent students.

Taking inital summaries of the dataset presented some large outliers,
particularly in the expenditure variables. As a result, Average Teacher
Salary and Proportion of Teacher and Support Staff Salary Spending to
Total Personnel Expenditure were both normalized.

<table>

<caption>

Summary Statistics

</caption>

<thead>

<tr>

<th style="text-align:left;">

</th>

<th style="text-align:left;">

Mean

</th>

<th style="text-align:left;">

SD

</th>

<th style="text-align:left;">

Min

</th>

<th style="text-align:left;">

Max

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

Total Enrollment

</td>

<td style="text-align:left;">

584.256

</td>

<td style="text-align:left;">

452.154

</td>

<td style="text-align:left;">

10.000

</td>

<td style="text-align:left;">

14286.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Chronic Absent Proportion

</td>

<td style="text-align:left;">

0.151

</td>

<td style="text-align:left;">

0.127

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Pupil to Teacher Ratio

</td>

<td style="text-align:left;">

15.618

</td>

<td style="text-align:left;">

5.631

</td>

<td style="text-align:left;">

0.167

</td>

<td style="text-align:left;">

489.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Minority Proportion

</td>

<td style="text-align:left;">

0.475

</td>

<td style="text-align:left;">

0.323

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Free Lunch Program Proportion

</td>

<td style="text-align:left;">

0.526

</td>

<td style="text-align:left;">

0.269

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Limited English Proportion

</td>

<td style="text-align:left;">

0.102

</td>

<td style="text-align:left;">

0.147

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.211

</td>

</tr>

<tr>

<td style="text-align:left;">

Average Teacher Salary

</td>

<td style="text-align:left;">

62260.695

</td>

<td style="text-align:left;">

140663.637

</td>

<td style="text-align:left;">

0.250

</td>

<td style="text-align:left;">

23991287.736

</td>

</tr>

<tr>

<td style="text-align:left;">

Normalized Average Teacher Salary

</td>

<td style="text-align:left;">

0.003

</td>

<td style="text-align:left;">

0.006

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Per Pupil Expenditure

</td>

<td style="text-align:left;">

7382.831

</td>

<td style="text-align:left;">

31548.287

</td>

<td style="text-align:left;">

0.002

</td>

<td style="text-align:left;">

7238598.800

</td>

</tr>

<tr>

<td style="text-align:left;">

Ratio of Inexperienced Teachers to 2+ Year Teachers

</td>

<td style="text-align:left;">

0.117

</td>

<td style="text-align:left;">

0.124

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

2.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Proportion of Teacher and Support Staff Salary Spending to Total
Personnel Expenditure

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

0.005

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

1.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Ratio of Support Staff to Teachers

</td>

<td style="text-align:left;">

0.081

</td>

<td style="text-align:left;">

2.023

</td>

<td style="text-align:left;">

0.000

</td>

<td style="text-align:left;">

540.790

</td>

</tr>

</tbody>

</table>

The summary statistics demonstrate some severe outliers within the
dataset. The self-reported nature of the data could account for these
extreme values. Despite the extremities, the mean values of the selected
variables seem to be reasonable.

Using this data set, the models will test for the impact of school
resources, as measured by Per Pupil Expenditure, Teacher Inexperience,
Average Teach Salary, Proportion of Personnel Expenditure on Teachers
and Support Staff and the Proportion of Support Staff to Teachers on
rates of Chronic Absenteeism. The expenditure on teachers and support
staff is being used as a proxy for teacher quality, as the data sets did
not have information on teacher qualifications other than whether they
meet state certification standards.

The hypothesis is: that added school resources should negatively
correlate with the chronic absentee rate, in that more experienced
teachers, quality teachers and added support staff create an engaging,
positive environment for their students to be in.

#### Methodology

To test the dependent variable, rate of chronic absenteeism, the
ordinary least squares regression will be run first. The model will
estimate Chronic Absentee Proportion as a function of the resource
effects, Per Pupil Expenditure, Teacher Inexperience, Average Teach
Salary, Proportion of Personnel Expenditure on Teachers and Support
Staff and the Proportion of Support Staff to Teachers, with student
effect controls, Pupil to Teacher Ration, Minority Proportion, Free
Lunch Eligible Proportion, Limited English Proficiency Proportion and
Type of School (Special Education, Charter, Magnet, Alternative. Schools
not listed as one of these four categories are other graded and ungraded
schools).

Then a Lasso Model will be run using the same variables to test which
have the least influence on Chronic Absenteeism. After the Lasso
Regression is run, a second OLS regression with the least influential
variables removed will be run.

Lastly, an OLS regression with interactions on the remaining variables
will be run to test the impact of school type on the remaining
variables.

#### Results

**OLS**

<table>

<thead>

<tr>

<th style="text-align:left;">

</th>

<th style="text-align:right;">

Estimate

</th>

<th style="text-align:right;">

Std. Error

</th>

<th style="text-align:right;">

t value

</th>

<th style="text-align:right;">

Pr(\>|t|)

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

(Intercept)

</td>

<td style="text-align:right;">

0.048

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

30.875

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm

</td>

<td style="text-align:right;">

0.104

</td>

<td style="text-align:right;">

0.070

</td>

<td style="text-align:right;">

1.495

</td>

<td style="text-align:right;">

0.135

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachInexp

</td>

<td style="text-align:right;">

0.056

</td>

<td style="text-align:right;">

0.003

</td>

<td style="text-align:right;">

16.233

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1

</td>

<td style="text-align:right;">

0.174

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

42.847

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Alternative1

</td>

<td style="text-align:right;">

0.372

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

87.857

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Magnet1

</td>

<td style="text-align:right;">

\-0.006

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

\-3.149

</td>

<td style="text-align:right;">

0.002

</td>

</tr>

<tr>

<td style="text-align:left;">

Charter1

</td>

<td style="text-align:right;">

0.012

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

5.914

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PPE

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.471

</td>

<td style="text-align:right;">

0.638

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachSupSalPropNorm

</td>

<td style="text-align:right;">

\-0.001

</td>

<td style="text-align:right;">

0.075

</td>

<td style="text-align:right;">

\-0.015

</td>

<td style="text-align:right;">

0.988

</td>

</tr>

<tr>

<td style="text-align:left;">

ETOTAL

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

20.954

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PupilTeachRatio

</td>

<td style="text-align:right;">

\-0.001

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-8.596

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

EMinProp

</td>

<td style="text-align:right;">

0.031

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

15.703

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

frplProp

</td>

<td style="text-align:right;">

0.173

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

86.476

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

LEPProp

</td>

<td style="text-align:right;">

\-0.171

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

\-48.613

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

</tbody>

</table>

The initial OLS Regression demonstrates that the expenditure based
teacher effect variables have a nonstatistical relationship with chronic
absentee rates. The remaining variables, while demonstrating
statistically significant correlations, generally have low correlations
on chronic absenteeism. It is of interest that Special Education schools
and Alternative schools have the largest correlation, both positive, on
the rate of chronic absenteeism. Despite potentially having access to
greater resources to help serve their students, these two results
demonstrate the issues of endogeneity with assessing school resources -
are the resources provided to the students to help improve their
educational opportunities, or are added resources needed to provide
particular cohorts with an acceptable education experience?

Here are some plots of Minority Proportion correlation, Free and Reduced
Price Lunch Proportion correlation and Inexperience Teacher Ratio
correlation. ![EMinPropOLS](./EMinPropOLS.png)

![FRPLPropOLS](./FRPLPropOLS.png)

![TeachInexpOLS](./TeachInexpOLS.png)
![](FProjv2_files/figure-gfm/OLS%20Plots-1.png)<!-- -->
![](FProjv2_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->
![](FProjv2_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

**LASSO**

<table>

<thead>

<tr>

<th style="text-align:left;">

</th>

<th style="text-align:right;">

x

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachInexp

</td>

<td style="text-align:right;">

0.006

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED

</td>

<td style="text-align:right;">

0.167

</td>

</tr>

<tr>

<td style="text-align:left;">

Alternative

</td>

<td style="text-align:right;">

0.367

</td>

</tr>

<tr>

<td style="text-align:left;">

Magnet

</td>

<td style="text-align:right;">

\-0.009

</td>

</tr>

<tr>

<td style="text-align:left;">

Charter

</td>

<td style="text-align:right;">

0.011

</td>

</tr>

<tr>

<td style="text-align:left;">

PPE

</td>

<td style="text-align:right;">

0.003

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachSupSalPropNorm

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

ETOTAL

</td>

<td style="text-align:right;">

0.009

</td>

</tr>

<tr>

<td style="text-align:left;">

PupilTeachRatio

</td>

<td style="text-align:right;">

\-0.003

</td>

</tr>

<tr>

<td style="text-align:left;">

EMinProp

</td>

<td style="text-align:right;">

0.010

</td>

</tr>

<tr>

<td style="text-align:left;">

frplProp

</td>

<td style="text-align:right;">

0.047

</td>

</tr>

<tr>

<td style="text-align:left;">

LEPProp

</td>

<td style="text-align:right;">

\-0.025

</td>

</tr>

</tbody>

</table>

![LassoChart](./LassoChart.png)

The Lasso Model confirms the results of the initial OLS model. THe
expenditure related teacher variables have the least impact on
estimating the chronic absentee rate. School type remains interesting.
The Magnet and Charter schools appear to have little impact on chronic
absentee rates.

The second OLS model removes two of the school types, leaving the
expenditure teacher variables so as not to change the equation
drastically.

<table>

<thead>

<tr>

<th style="text-align:left;">

</th>

<th style="text-align:right;">

Estimate

</th>

<th style="text-align:right;">

Std. Error

</th>

<th style="text-align:right;">

t value

</th>

<th style="text-align:right;">

Pr(\>|t|)

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

(Intercept)

</td>

<td style="text-align:right;">

0.048

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

30.757

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm

</td>

<td style="text-align:right;">

0.099

</td>

<td style="text-align:right;">

0.070

</td>

<td style="text-align:right;">

1.412

</td>

<td style="text-align:right;">

0.158

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachInexp

</td>

<td style="text-align:right;">

0.061

</td>

<td style="text-align:right;">

0.003

</td>

<td style="text-align:right;">

17.917

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1

</td>

<td style="text-align:right;">

0.174

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

42.858

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Alternative1

</td>

<td style="text-align:right;">

0.372

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

87.966

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PPE

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.558

</td>

<td style="text-align:right;">

0.577

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachSupSalPropNorm

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.075

</td>

<td style="text-align:right;">

\-0.004

</td>

<td style="text-align:right;">

0.997

</td>

</tr>

<tr>

<td style="text-align:left;">

ETOTAL

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

20.263

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PupilTeachRatio

</td>

<td style="text-align:right;">

\-0.001

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-8.126

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

EMinProp

</td>

<td style="text-align:right;">

0.031

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

16.351

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

frplProp

</td>

<td style="text-align:right;">

0.173

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

86.403

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

LEPProp

</td>

<td style="text-align:right;">

\-0.171

</td>

<td style="text-align:right;">

0.003

</td>

<td style="text-align:right;">

\-49.004

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

</tbody>

</table>

Having remove the Magnet and Charter school types, expenditure teacher
variables still have a nonstatistical relationship to chronic absentee
rates. The normalized average teacher salary has less of a correlation
at even less significance. Teacher Inexperience ratio increased its
level of correlation by 1.5 standard deviations. All other variables
remained constant.

To test the impact of school type against the remaining variables, the
last OLS regression interacts the Special Education and Alternative
school dummary variables against the student and teacher effects
variables.

<table>

<thead>

<tr>

<th style="text-align:left;">

</th>

<th style="text-align:right;">

Estimate

</th>

<th style="text-align:right;">

Std. Error

</th>

<th style="text-align:right;">

t value

</th>

<th style="text-align:right;">

Pr(\>|t|)

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

(Intercept)

</td>

<td style="text-align:right;">

0.045

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

27.809

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm

</td>

<td style="text-align:right;">

0.056

</td>

<td style="text-align:right;">

0.069

</td>

<td style="text-align:right;">

0.811

</td>

<td style="text-align:right;">

0.418

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1

</td>

<td style="text-align:right;">

0.154

</td>

<td style="text-align:right;">

0.015

</td>

<td style="text-align:right;">

10.477

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachInexp

</td>

<td style="text-align:right;">

0.062

</td>

<td style="text-align:right;">

0.003

</td>

<td style="text-align:right;">

18.026

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PPE

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

4.440

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachSupSalPropNorm

</td>

<td style="text-align:right;">

\-0.001

</td>

<td style="text-align:right;">

0.075

</td>

<td style="text-align:right;">

\-0.008

</td>

<td style="text-align:right;">

0.993

</td>

</tr>

<tr>

<td style="text-align:left;">

ETOTAL

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

21.577

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PupilTeachRatio

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-5.391

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

EMinProp

</td>

<td style="text-align:right;">

0.027

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

13.913

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

frplProp

</td>

<td style="text-align:right;">

0.173

</td>

<td style="text-align:right;">

0.002

</td>

<td style="text-align:right;">

86.273

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

LEPProp

</td>

<td style="text-align:right;">

\-0.170

</td>

<td style="text-align:right;">

0.004

</td>

<td style="text-align:right;">

\-48.401

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

Alternative1

</td>

<td style="text-align:right;">

0.180

</td>

<td style="text-align:right;">

0.016

</td>

<td style="text-align:right;">

10.977

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm:SPED1

</td>

<td style="text-align:right;">

3.428

</td>

<td style="text-align:right;">

2.428

</td>

<td style="text-align:right;">

1.412

</td>

<td style="text-align:right;">

0.158

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:TeachInexp

</td>

<td style="text-align:right;">

0.079

</td>

<td style="text-align:right;">

0.022

</td>

<td style="text-align:right;">

3.549

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:PPE

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-4.989

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:TeachSupSalPropNorm

</td>

<td style="text-align:right;">

\-61146.246

</td>

<td style="text-align:right;">

15851.537

</td>

<td style="text-align:right;">

\-3.857

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:ETOTAL

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-11.472

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:PupilTeachRatio

</td>

<td style="text-align:right;">

\-0.002

</td>

<td style="text-align:right;">

0.001

</td>

<td style="text-align:right;">

\-4.274

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:EMinProp

</td>

<td style="text-align:right;">

0.160

</td>

<td style="text-align:right;">

0.018

</td>

<td style="text-align:right;">

9.171

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:frplProp

</td>

<td style="text-align:right;">

0.003

</td>

<td style="text-align:right;">

0.018

</td>

<td style="text-align:right;">

0.151

</td>

<td style="text-align:right;">

0.880

</td>

</tr>

<tr>

<td style="text-align:left;">

SPED1:LEPProp

</td>

<td style="text-align:right;">

\-0.055

</td>

<td style="text-align:right;">

0.039

</td>

<td style="text-align:right;">

\-1.401

</td>

<td style="text-align:right;">

0.161

</td>

</tr>

<tr>

<td style="text-align:left;">

AvgTeachSalNorm:Alternative1

</td>

<td style="text-align:right;">

26.307

</td>

<td style="text-align:right;">

2.429

</td>

<td style="text-align:right;">

10.830

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachInexp:Alternative1

</td>

<td style="text-align:right;">

\-0.088

</td>

<td style="text-align:right;">

0.023

</td>

<td style="text-align:right;">

\-3.894

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PPE:Alternative1

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-4.497

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

TeachSupSalPropNorm:Alternative1

</td>

<td style="text-align:right;">

\-170243.675

</td>

<td style="text-align:right;">

44127.423

</td>

<td style="text-align:right;">

\-3.858

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

ETOTAL:Alternative1

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

\-5.485

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

PupilTeachRatio:Alternative1

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

0.000

</td>

<td style="text-align:right;">

1.411

</td>

<td style="text-align:right;">

0.158

</td>

</tr>

<tr>

<td style="text-align:left;">

EMinProp:Alternative1

</td>

<td style="text-align:right;">

0.150

</td>

<td style="text-align:right;">

0.017

</td>

<td style="text-align:right;">

8.944

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

frplProp:Alternative1

</td>

<td style="text-align:right;">

0.103

</td>

<td style="text-align:right;">

0.020

</td>

<td style="text-align:right;">

5.132

</td>

<td style="text-align:right;">

0.000

</td>

</tr>

<tr>

<td style="text-align:left;">

LEPProp:Alternative1

</td>

<td style="text-align:right;">

0.086

</td>

<td style="text-align:right;">

0.032

</td>

<td style="text-align:right;">

2.726

</td>

<td style="text-align:right;">

0.006

</td>

</tr>

</tbody>

</table>

The interaction model demonstrates large changes in the correlation of
the normalized expenditure variables Average Teacher Salary and Teacher
and Support Staff Salary as a Proportion of Personnel Expenditure, when
they are interacted with both Special Education and Alternative school
type variables. Free Lunch Eligible Proportion and Limited English
Proportion variables also change significantly when interacted with the
Special Education variable, both taking on insignificant p-values,
suggesting that Special Education schools may have cohorts with low
proportions of free lunch eligible and limited English proficient
students. We see movements in the same direction of those two variables
when interacted with the Alternative school variable, though the
movements are to the opposite degree. Both coefficients remain
statistically significant. The other variables in the model do not
change significantly. This suggests that Special Education and
Alternative schools have greater impacts on chronic absenteeism due to
expenditure factors than other schools. Specifically, the coefficients
suggests that increased spending on Support Staff is beneficial, given
that Average Teacher Salary has positive correlation with the interacted
Special Education and Alternative school variables while the Proportion
of Teacher and Support Staff Salary to Personnel Expenditure has a
negative correlation. The implication is that support staff members can
provide better outcomes for students in these environments than just
regular teachers.

#### Conclusion

The analysis of school resources in these models, in terms of
expenditure and non-expenditure measures, implies that there is little
correlation with rates of chronic absenteeism. Student factors have more
statistically significant relationships with rates of chronic
absenteeism but the values of correlation coefficients appear to small
to be real world practical. There are issues of endogeneity within the
line of inquiry. The first regards proportions of students in poverty.
Cohorts with higher proportions of children in poverty, here accounted
for through the free lunch program variable, could have higher rates of
Limited English Proficiency students. They may also face less engagement
from other members of their cohort and the teacher body, presenting
issues of disengagement, hostility and lack of support prompting them to
be less likely to go to school. Similarly, accounting for Teacher
Inexperience Ratio is a less than ideal measure for teacher quality.
Teachers with more experience do have advantages for students but
experience does not always translate to quality.

It would be an ideal outcome for policy makers to be presented with the
chance to put money towards an initiative or program and know that it
will lead to a good outcome. With chronic absenteeism, which can be an
indicator for later educational outcomes, this does not appear to be the
case. There are too many confounding variables outside the realm of
school resources to have an instantaneous impact on reducing rates.
Providing support staff, engaging parents and building positive learning
environments is but one piece of the education puzzle. Chronic
absenteeism appears to be more influenced by background factors. Given
the impacts that chronic absenteeism can have on an individual’s
learning an education, to the extent of damaging matriculation
opportunities, it would be well worth pursuing programs within poor and
minority communities to reduce the 16% of American school students
chronically absent each year (U.S.Department of Education 2019).

#### Bibliography

Balfanz, R. (2016). Missing school matters. The Phi Delta Kappan, 98(2),
8-13. Retrieved December 1, 2020, from
<http://www.jstor.org/stable/24893461>

Branham, D. (2004), The Wise Man Builds His House Upon the Rock: The
Effects of Inadequate School Building Infrastructure on Student
Attendance. Social Science Quarterly, 85: 1112-1128.
<https://doi.org/10.1111/j.0038-4941.2004.00266.x>

Gershenson, S. (2016). Linking Teacher Quality, Student Attendance, and
Student Achievement. Education Finance and Policy 2016 11:2, 125-149.
Accessed November 29, 2020,
<https://www.mitpressjournals.org/doi/full/10.1162/EDFP_a_00180>

Grosskopf, S., Hayes, K., Taylor, L.L. et al. (2015). Centralized or
decentralized control of school resources? A network model. J Prod Anal
43, 139–150. Accessed December 1, 2020,
<https://doi.org/10.1007/s11123-013-0379-2>

Hanushek, E. (1989). The Impact of Differential Expenditures on School
Performance. Educational Researcher, 18(4), 45-62. Retrieved December
12, 2020, from <http://www.jstor.org/stable/1176650>

Hedges, L., Pigott, T., Polanin, J., Ryan, A., Tocci, C., & Williams, R.
(2016). The Question of School Resources and Student Achievement: A
History and Reconsideration. Review of Research in Education, 40,
143-168. Retrieved December 4, 2020, from
<http://www.jstor.org/stable/44668621>

Houtenville, A., & Conway, K. (2008). Parental Effort, School Resources,
and Student Achievement. The Journal of Human Resources, 43(2), 437-453.
Retrieved December 1, 2020, from <http://www.jstor.org/stable/40057353>

Iatarola, P., & Rubenstein, R. (2007). New Stakes and Standards, Same
Ol’ Spending? Evidence from New York City High Schools. Education
Finance and Policy, 2(1), 74-99. Retrieved December 4, 2020, from
<http://www.jstor.org/stable/educfinapoli.2.1.74>

Lee, T., Cornell, D., Gregory, A., & Fan, X. (2011). High Suspension
Schools and Dropout Rates for Black and White Students. Education and
Treatment of Children, 34(2), 167-192. Retrieved December 4, 2020, from
<http://www.jstor.org/stable/42900581>

Owens, A. (2010). Neighborhoods and Schools as Competing and Reinforcing
Contexts for Educational Attainment. Sociology of Education, 83(4),
287-311. Retrieved December 4, 2020, from
<http://www.jstor.org/stable/25746205>

Reardon, S.F., Kalogrides, D., & Shores, K. (2019). The Geography of
Racial/Ethnic Test Score Gaps. The American Journal of Sociology,
124(4). Accessed December 1, 2020,
<https://cepa.stanford.edu/sites/default/files/wp16-10-v201604.pdf>

United States Department of Education. (2019). Accessed December 16,
2020, <https://www2.ed.gov/datastory/chronicabsenteeism.html#intro>

**Data** CRDC (the EDFacts Supplement is included in the CRDC Download)
<https://www2.ed.gov/about/offices/list/ocr/docs/crdc-2017-18.html> CCD
<https://nces.ed.gov/ccd/files.asp#Fiscal:2,LevelId:7,SchoolYearId:32,Page:1>
