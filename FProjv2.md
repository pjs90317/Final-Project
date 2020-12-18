ECOB2000 Final Project
================
Patrick Sinclair

    ## Loading required package: knitr

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

    ## Loading required package: car

    ## Loading required package: carData

    ## 
    ## Attaching package: 'car'

    ## The following object is masked from 'package:dplyr':
    ## 
    ##     recode

    ## Loading required package: lmtest

    ## Loading required package: zoo

    ## 
    ## Attaching package: 'zoo'

    ## The following objects are masked from 'package:base':
    ## 
    ##     as.Date, as.Date.numeric

    ## Loading required package: sandwich

    ## Loading required package: survival

    ## 
    ## Please cite as:

    ##  Hlavac, Marek (2018). stargazer: Well-Formatted Regression and Summary Statistics Tables.

    ##  R package version 5.2.2. https://CRAN.R-project.org/package=stargazer

    ## Warning: package 'kableExtra' was built under R version 4.0.3

    ## 
    ## Attaching package: 'kableExtra'

    ## The following object is masked from 'package:dplyr':
    ## 
    ##     group_rows

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

``` r
absent1 <- lm(AbsentProp ~ AvgTeachSalNorm + TeachInexp + SPED + Alternative + Magnet + Charter + PPE + TeachSupSalPropNorm + ETOTAL + PupilTeachRatio + EMinProp + frplProp + LEPProp, data = useData3)
summary(absent1)
```

    ## 
    ## Call:
    ## lm(formula = AbsentProp ~ AvgTeachSalNorm + TeachInexp + SPED + 
    ##     Alternative + Magnet + Charter + PPE + TeachSupSalPropNorm + 
    ##     ETOTAL + PupilTeachRatio + EMinProp + frplProp + LEPProp, 
    ##     data = useData3)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -0.69113 -0.05964 -0.02080  0.03617  0.89469 
    ## 
    ## Coefficients:
    ##                       Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)          4.777e-02  1.547e-03  30.875  < 2e-16 ***
    ## AvgTeachSalNorm      1.043e-01  6.976e-02   1.495  0.13505    
    ## TeachInexp           5.626e-02  3.466e-03  16.233  < 2e-16 ***
    ## SPED1                1.741e-01  4.063e-03  42.847  < 2e-16 ***
    ## Alternative1         3.719e-01  4.233e-03  87.857  < 2e-16 ***
    ## Magnet1             -6.132e-03  1.947e-03  -3.149  0.00164 ** 
    ## Charter1             1.164e-02  1.968e-03   5.914 3.36e-09 ***
    ## PPE                  6.136e-09  1.303e-08   0.471  0.63770    
    ## TeachSupSalPropNorm -1.096e-03  7.528e-02  -0.015  0.98838    
    ## ETOTAL               2.076e-05  9.906e-07  20.954  < 2e-16 ***
    ## PupilTeachRatio     -6.578e-04  7.652e-05  -8.596  < 2e-16 ***
    ## EMinProp             3.070e-02  1.955e-03  15.703  < 2e-16 ***
    ## frplProp             1.733e-01  2.004e-03  86.476  < 2e-16 ***
    ## LEPProp             -1.710e-01  3.517e-03 -48.613  < 2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 0.1093 on 71653 degrees of freedom
    ## Multiple R-squared:  0.2574, Adjusted R-squared:  0.2572 
    ## F-statistic:  1910 on 13 and 71653 DF,  p-value: < 2.2e-16

``` r
# stargazer(absent1, type = "text")
plot(absent1)
```

![](FProjv2_files/figure-gfm/Initial%20OLS%20Regression-1.png)<!-- -->![](FProjv2_files/figure-gfm/Initial%20OLS%20Regression-2.png)<!-- -->![](FProjv2_files/figure-gfm/Initial%20OLS%20Regression-3.png)<!-- -->![](FProjv2_files/figure-gfm/Initial%20OLS%20Regression-4.png)<!-- -->

``` r
absentcoefs <- kable(summary(absent1)$coef, digits=3)
# save_kable(absentcoefs, file = "AbsentOLSCoefs.png")
```

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

![](FProjv2_files/figure-gfm/OLS%20Plots-1.png)<!-- -->

``` r
attach(graphset)
```

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

``` r
# png(filename = "./FRPLPropOLS.png")
plot(AbsentProp ~ jitter(frplProp, factor = 0.0), pch = 15, col = rgb(0.5, 0.8, 0, alpha = 0.8), ylim = c(0,1), xlim = c(0,1), xlab="FRPL Prop", data = graphset)
abspredictfrpl <- data.frame(AvgTeachSalNorm = 0.0015, TeachInexp = 0.5, SPED, Alternative, Magnet, Charter, PPE = 7500, ETOTAL = 250, PupilTeachRatio = 15, EMinProp = 0.5, (frplProp >= 0.1 & frplProp <= 0.9), LEPProp = 0.1, TeachSupSalPropNorm = 0.05)
abspredictfrpl$yhat <- predict(absent1, newdata = abspredictfrpl)
lines(yhat ~ frplProp, data = abspredictfrpl, col = "Blue")
legend("topleft", "Free and Reduced Price Lunch RL", col = "Blue", lty = 1, bty = "n")
```

![](FProjv2_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

``` r
# dev.off()
detach()
```

``` r
attach(graphset)
```

    ## The following object is masked _by_ .GlobalEnv:
    ## 
    ##     frpl

``` r
# png(filename = "./TeachInexpOLS.png")
plot(AbsentProp ~ jitter(TeachInexp, factor = 0.0), pch = 15, col = rgb(0.5, 0.8, 0, alpha = 0.8), ylim = c(0,1), xlim = c(0,1), xlab="Inexperienced Teacher Proportion", data = graphset)
abspredictinexp <- data.frame(AvgTeachSalNorm = 0.0015, (TeachInexp >= 0.05 & TeachInexp <= 1), SPED, Alternative, Magnet, Charter, PPE = 6500, ETOTAL = 250, PupilTeachRatio = 15, EMinProp = 0.5, frplProp = 0.05, LEPProp = 0.1, TeachSupSalPropNorm = 0.05)
abspredictinexp$yhat <- predict(absent1, newdata = abspredictinexp)
lines(yhat ~ TeachInexp, data = abspredictinexp, col = "Red")
legend("topleft", "Teacher Inexperience Ration RL", col = "Red", lty = 1, bty = "n")
```

![](FProjv2_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

``` r
# dev.off()
detach()
```

**LASSO**

    ## Loading required package: standardize

    ## Warning: package 'standardize' was built under R version 4.0.3

    ## Registered S3 methods overwritten by 'lme4':
    ##   method                          from
    ##   cooks.distance.influence.merMod car 
    ##   influence.merMod                car 
    ##   dfbeta.influence.merMod         car 
    ##   dfbetas.influence.merMod        car

    ## [1] 71667

    ## Loading required package: vip

    ## Warning: package 'vip' was built under R version 4.0.3

    ## 
    ## Attaching package: 'vip'

    ## The following object is masked from 'package:utils':
    ## 
    ##     vi

    ## Loading required package: glmnet

    ## Warning: package 'glmnet' was built under R version 4.0.3

    ## Loading required package: Matrix

    ## Loaded glmnet 4.0-2

![](FProjv2_files/figure-gfm/Standardize%20Data%20and%20Lasso%20Regression-1.png)<!-- -->![](FProjv2_files/figure-gfm/Standardize%20Data%20and%20Lasso%20Regression-2.png)<!-- -->![](FProjv2_files/figure-gfm/Standardize%20Data%20and%20Lasso%20Regression-3.png)<!-- -->

    ## 
    ## Call:  glmnet(x = as.matrix(sobj$data[, -1]), y = sobj$data$AbsentProp,      alpha = 1) 
    ## 
    ##    Df  %Dev   Lambda
    ## 1   0  0.00 0.043990
    ## 2   1  2.02 0.040080
    ## 3   2  4.13 0.036520
    ## 4   2  6.80 0.033280
    ## 5   2  9.01 0.030320
    ## 6   2 10.85 0.027630
    ## 7   2 12.38 0.025170
    ## 8   2 13.65 0.022940
    ## 9   2 14.70 0.020900
    ## 10  2 15.58 0.019040
    ## 11  3 16.54 0.017350
    ## 12  3 17.45 0.015810
    ## 13  3 18.20 0.014400
    ## 14  3 18.82 0.013120
    ## 15  3 19.33 0.011960
    ## 16  4 20.10 0.010900
    ## 17  4 20.75 0.009928
    ## 18  4 21.29 0.009046
    ## 19  5 21.75 0.008243
    ## 20  5 22.17 0.007510
    ## 21  6 22.60 0.006843
    ## 22  7 23.00 0.006235
    ## 23  7 23.36 0.005681
    ## 24  7 23.65 0.005177
    ## 25  7 23.90 0.004717
    ## 26  7 24.10 0.004298
    ## 27  8 24.27 0.003916
    ## 28  8 24.43 0.003568
    ## 29  9 24.55 0.003251
    ## 30  9 24.66 0.002962
    ## 31  9 24.76 0.002699
    ## 32 10 24.83 0.002459
    ## 33 10 24.91 0.002241
    ## 34 10 24.96 0.002042
    ## 35 10 25.01 0.001860
    ## 36 10 25.05 0.001695
    ## 37 11 25.09 0.001545
    ## 38 11 25.12 0.001407
    ## 39 11 25.15 0.001282
    ## 40 11 25.17 0.001168
    ## 41 11 25.19 0.001065
    ## 42 11 25.21 0.000970
    ## 43 11 25.22 0.000884
    ## 44 11 25.23 0.000805
    ## 45 11 25.24 0.000734
    ## 46 11 25.24 0.000669
    ## 47 11 25.25 0.000609
    ## 48 11 25.26 0.000555
    ## 49 11 25.26 0.000506
    ## 50 11 25.26 0.000461
    ## 51 12 25.27 0.000420
    ## 52 12 25.27 0.000383
    ## 53 12 25.27 0.000349
    ## 54 12 25.27 0.000318
    ## 55 12 25.27 0.000289
    ## 56 12 25.28 0.000264
    ## 57 12 25.28 0.000240
    ## 58 12 25.28 0.000219
    ## 59 12 25.28 0.000199
    ## 60 13 25.28 0.000182
    ## 61 13 25.28 0.000166
    ## 62 13 25.28 0.000151
    ## 63 13 25.28 0.000138
    ## 64 13 25.28 0.000125
    ## 65 13 25.28 0.000114

    ## [1] 0.0004608305

![](FProjv2_files/figure-gfm/Standardize%20Data%20and%20Lasso%20Regression-4.png)<!-- -->

    ## [1] -7.68248

    ## 14 x 1 sparse Matrix of class "dgCMatrix"
    ##                                1
    ## (Intercept)          1.204979222
    ## AvgTeachSalNorm      .          
    ## TeachInexp           0.005558872
    ## SPED                -0.164163234
    ## Alternative         -0.363279450
    ## Magnet               0.007094042
    ## Charter             -0.009602536
    ## PPE                  0.002995820
    ## TeachSupSalPropNorm  .          
    ## ETOTAL               0.008103821
    ## PupilTeachRatio     -0.002460466
    ## EMinProp             0.009644964
    ## frplProp             0.046299050
    ## LEPProp             -0.024081537

![](FProjv2_files/figure-gfm/Standardize%20Data%20and%20Lasso%20Regression-5.png)<!-- -->

    ## 
    ## Call:
    ## lm(formula = AbsentProp ~ AvgTeachSalNorm + TeachInexp + SPED + 
    ##     Alternative + PPE + TeachSupSalPropNorm + ETOTAL + PupilTeachRatio + 
    ##     EMinProp + frplProp + LEPProp, data = useData3)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -0.68039 -0.05982 -0.02091  0.03610  0.89474 
    ## 
    ## Coefficients:
    ##                       Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)          4.757e-02  1.547e-03  30.757  < 2e-16 ***
    ## AvgTeachSalNorm      9.852e-02  6.977e-02   1.412    0.158    
    ## TeachInexp           6.063e-02  3.384e-03  17.917  < 2e-16 ***
    ## SPED1                1.742e-01  4.064e-03  42.858  < 2e-16 ***
    ## Alternative1         3.724e-01  4.233e-03  87.966  < 2e-16 ***
    ## PPE                  7.279e-09  1.303e-08   0.558    0.577    
    ## TeachSupSalPropNorm -2.686e-04  7.531e-02  -0.004    0.997    
    ## ETOTAL               1.993e-05  9.837e-07  20.263  < 2e-16 ***
    ## PupilTeachRatio     -6.202e-04  7.631e-05  -8.126  4.5e-16 ***
    ## EMinProp             3.123e-02  1.910e-03  16.351  < 2e-16 ***
    ## frplProp             1.726e-01  1.998e-03  86.403  < 2e-16 ***
    ## LEPProp             -1.714e-01  3.499e-03 -49.004  < 2e-16 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 0.1093 on 71655 degrees of freedom
    ## Multiple R-squared:  0.2569, Adjusted R-squared:  0.2568 
    ## F-statistic:  2252 on 11 and 71655 DF,  p-value: < 2.2e-16

![](FProjv2_files/figure-gfm/OLS%20Lasso%20Remove%20Varb-1.png)<!-- -->![](FProjv2_files/figure-gfm/OLS%20Lasso%20Remove%20Varb-2.png)<!-- -->![](FProjv2_files/figure-gfm/OLS%20Lasso%20Remove%20Varb-3.png)<!-- -->![](FProjv2_files/figure-gfm/OLS%20Lasso%20Remove%20Varb-4.png)<!-- -->

    ## 
    ## Call:
    ## lm(formula = AbsentProp ~ (AvgTeachSalNorm * SPED) + (TeachInexp * 
    ##     SPED) + (PPE * SPED) + (TeachSupSalPropNorm * SPED) + (ETOTAL * 
    ##     SPED) + (PupilTeachRatio * SPED) + (EMinProp * SPED) + (frplProp * 
    ##     SPED) + (LEPProp * SPED) + (AvgTeachSalNorm * Alternative) + 
    ##     (TeachInexp * Alternative) + (PPE * Alternative) + (TeachSupSalPropNorm * 
    ##     Alternative) + (ETOTAL * Alternative) + (PupilTeachRatio * 
    ##     Alternative) + (EMinProp * Alternative) + (frplProp * Alternative) + 
    ##     (LEPProp * Alternative), data = useData3)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -0.77612 -0.05964 -0.02107  0.03592  0.89715 
    ## 
    ## Coefficients:
    ##                                    Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)                       4.453e-02  1.601e-03  27.809  < 2e-16 ***
    ## AvgTeachSalNorm                   5.630e-02  6.946e-02   0.811 0.417634    
    ## SPED1                             1.542e-01  1.472e-02  10.477  < 2e-16 ***
    ## TeachInexp                        6.207e-02  3.443e-03  18.026  < 2e-16 ***
    ## PPE                               1.172e-07  2.640e-08   4.440 9.01e-06 ***
    ## TeachSupSalPropNorm              -6.249e-04  7.484e-02  -0.008 0.993338    
    ## ETOTAL                            2.120e-05  9.826e-07  21.577  < 2e-16 ***
    ## PupilTeachRatio                  -4.303e-04  7.982e-05  -5.391 7.04e-08 ***
    ## EMinProp                          2.679e-02  1.925e-03  13.913  < 2e-16 ***
    ## frplProp                          1.734e-01  2.010e-03  86.273  < 2e-16 ***
    ## LEPProp                          -1.701e-01  3.515e-03 -48.401  < 2e-16 ***
    ## Alternative1                      1.803e-01  1.642e-02  10.977  < 2e-16 ***
    ## AvgTeachSalNorm:SPED1             3.428e+00  2.428e+00   1.412 0.158029    
    ## SPED1:TeachInexp                  7.937e-02  2.236e-02   3.549 0.000387 ***
    ## SPED1:PPE                        -1.514e-07  3.035e-08  -4.989 6.09e-07 ***
    ## SPED1:TeachSupSalPropNorm        -6.115e+04  1.585e+04  -3.857 0.000115 ***
    ## SPED1:ETOTAL                     -2.182e-04  1.902e-05 -11.472  < 2e-16 ***
    ## SPED1:PupilTeachRatio            -2.446e-03  5.722e-04  -4.274 1.92e-05 ***
    ## SPED1:EMinProp                    1.605e-01  1.750e-02   9.171  < 2e-16 ***
    ## SPED1:frplProp                    2.729e-03  1.807e-02   0.151 0.879946    
    ## SPED1:LEPProp                    -5.468e-02  3.904e-02  -1.401 0.161325    
    ## AvgTeachSalNorm:Alternative1      2.631e+01  2.429e+00  10.830  < 2e-16 ***
    ## TeachInexp:Alternative1          -8.813e-02  2.263e-02  -3.894 9.88e-05 ***
    ## PPE:Alternative1                 -6.796e-07  1.511e-07  -4.497 6.89e-06 ***
    ## TeachSupSalPropNorm:Alternative1 -1.702e+05  4.413e+04  -3.858 0.000114 ***
    ## ETOTAL:Alternative1              -1.004e-04  1.830e-05  -5.485 4.15e-08 ***
    ## PupilTeachRatio:Alternative1      4.127e-04  2.924e-04   1.411 0.158121    
    ## EMinProp:Alternative1             1.496e-01  1.672e-02   8.944  < 2e-16 ***
    ## frplProp:Alternative1             1.029e-01  2.005e-02   5.132 2.87e-07 ***
    ## LEPProp:Alternative1              8.610e-02  3.159e-02   2.726 0.006420 ** 
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 0.1086 on 71637 degrees of freedom
    ## Multiple R-squared:  0.2663, Adjusted R-squared:  0.266 
    ## F-statistic: 896.4 on 29 and 71637 DF,  p-value: < 2.2e-16

![](FProjv2_files/figure-gfm/OLS%20Interactions-1.png)<!-- -->![](FProjv2_files/figure-gfm/OLS%20Interactions-2.png)<!-- -->![](FProjv2_files/figure-gfm/OLS%20Interactions-3.png)<!-- -->

    ## Warning in sqrt(crit * p * (1 - hh)/hh): NaNs produced
    
    ## Warning in sqrt(crit * p * (1 - hh)/hh): NaNs produced

![](FProjv2_files/figure-gfm/OLS%20Interactions-4.png)<!-- --> \#\#\#\#
Bibliography
