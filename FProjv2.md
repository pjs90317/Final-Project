ECOB2000 Final Project
================
Patrick Sinclair

    ## Warning in cbind(InitCAbsentee$COMBOKEY, InitEnrollment$COMBOKEY): number of
    ## rows of result is not a multiple of vector length (arg 1)

    ## # A tibble: 89,204 x 11
    ##    COMBOKEY SCH_FTETEACH_TOT SCH_FTETEACH_CE~ SCH_FTETEACH_NO~ SCH_FTETEACH_FY
    ##    <chr>               <dbl>            <dbl>            <dbl>           <dbl>
    ##  1 0100005~            39.3             39.3                 0               2
    ##  2 0100005~            78.2             71.2                 7               6
    ##  3 0100005~            41.4             41.4                 0               8
    ##  4 0100005~            52.8             52.8                 0               5
    ##  5 0100005~            29.4             29.4                 0               1
    ##  6 0100005~            71.0             71.0                 0               7
    ##  7 0100006~            18.2             18.2                 0               0
    ##  8 0100006~            32               31                   1               1
    ##  9 0100006~             7.65             7.65                0               0
    ## 10 0100006~            24.3             24.3                 0               3
    ## # ... with 89,194 more rows, and 6 more variables: SCH_FTETEACH_SY <dbl>,
    ## #   SCH_FTETEACH_ABSENT <dbl>, SCH_FTECOUNSELORS <dbl>,
    ## #   SCH_FTESERVICES_NUR <dbl>, SCH_FTESERVICES_PSY <dbl>,
    ## #   SCH_FTESERVICES_SOC <dbl>

### Introduction

#### Literature Review

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

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

![](FProjv2_files/figure-gfm/OLS%20Plots-1.png)<!-- -->

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

![](FProjv2_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

![](FProjv2_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

**LASSO**

#### Bibliography
