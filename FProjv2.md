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
achievement levels(Grosskopf et al. 2013). There is a subsection of the
literature that focuses on the impact and efficiency of educational
resources. Predominantly this research has sought to find correlation
between resource availability or allocation and educational attainment.

This paper uses the U.s. Department of Education 2017-18 Civil Rights
Data Collection, National Center for Education Statistics Common Core of
Data 2017-18 Lunch Program Eligibility Survey and the U.s. Department of
Education EDFacts Data Set 2017-18 Chronic Absenteeism Table (DG 814) to
test for a correlation between school resources and the rate of chronic
absenteeism in schools. Chronic absenteeism is defined as missing 15 or
more days of school (U.S. Department of Education, 2019). Chronic
absenteeism can have negative impacts on educational achievements across
all levels of education (Balfanz 2016).

#### Literature Review

The statistical literature on education outcomes has generally focused
on assessment scores and graduation rates as functions of cost and
socioeconomic inputs.

#### Data

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

#### Methodology

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

#### Bibliography

Balfanz, R. (2016). Missing school matters. The Phi Delta Kappan, 98(2),
8-13. Retrieved December 1, 2020, from
<http://www.jstor.org/stable/24893461>

Grosskopf, S., Hayes, K., Taylor, L.L. et al. (2015). Centralized or
decentralized control of school resources? A network model. J Prod Anal
43, 139–150. Accessed December 1, 2020,
<https://doi.org/10.1007/s11123-013-0379-2>

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
