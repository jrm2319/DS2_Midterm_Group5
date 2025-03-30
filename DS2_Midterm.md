Data Science 2 Midterm
================

    ## Loading required package: ggplot2

    ## Loading required package: lattice

<<<<<<< HEAD
    ## ── Attaching packages ────────────────────────────────────── tidymodels 1.3.0 ──
=======
    ## ── Attaching packages ────────────────────────────────────── tidymodels 1.2.0 ──
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee

    ## ✔ broom        1.0.7     ✔ rsample      1.2.1
    ## ✔ dials        1.4.0     ✔ tibble       3.2.1
    ## ✔ dplyr        1.1.4     ✔ tidyr        1.3.1
    ## ✔ infer        1.0.7     ✔ tune         1.2.1
    ## ✔ modeldata    1.4.0     ✔ workflows    1.1.4
    ## ✔ parsnip      1.3.0     ✔ workflowsets 1.1.0
    ## ✔ purrr        1.0.2     ✔ yardstick    1.3.2
    ## ✔ recipes      1.1.1

    ## ── Conflicts ───────────────────────────────────────── tidymodels_conflicts() ──
    ## ✖ purrr::discard()         masks scales::discard()
    ## ✖ dplyr::filter()          masks stats::filter()
    ## ✖ dplyr::lag()             masks stats::lag()
    ## ✖ purrr::lift()            masks caret::lift()
    ## ✖ yardstick::precision()   masks caret::precision()
    ## ✖ yardstick::recall()      masks caret::recall()
    ## ✖ yardstick::sensitivity() masks caret::sensitivity()
    ## ✖ yardstick::specificity() masks caret::specificity()
    ## ✖ recipes::step()          masks stats::step()
<<<<<<< HEAD
=======
    ## • Search for functions across packages at https://www.tidymodels.org/find/
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee

    ## Loading required package: nlme

    ## 
    ## Attaching package: 'nlme'

    ## The following object is masked from 'package:dplyr':
    ## 
    ##     collapse

    ## This is mgcv 1.9-1. For overview type 'help("mgcv-package")'.

    ## 
    ## Attaching package: 'pdp'

    ## The following object is masked from 'package:purrr':
    ## 
    ##     partial

    ## Loading required package: Formula

    ## Loading required package: plotmo

    ## Loading required package: plotrix

    ## 
    ## Attaching package: 'plotrix'

    ## The following object is masked from 'package:scales':
    ## 
    ##     rescale

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ forcats   1.0.0     ✔ readr     2.1.5
<<<<<<< HEAD
    ## ✔ lubridate 1.9.3     ✔ stringr   1.5.1
=======
    ## ✔ lubridate 1.9.4     ✔ stringr   1.5.1
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ readr::col_factor() masks scales::col_factor()
    ## ✖ nlme::collapse()    masks dplyr::collapse()
    ## ✖ purrr::discard()    masks scales::discard()
    ## ✖ dplyr::filter()     masks stats::filter()
    ## ✖ stringr::fixed()    masks recipes::fixed()
    ## ✖ dplyr::lag()        masks stats::lag()
    ## ✖ purrr::lift()       masks caret::lift()
    ## ✖ pdp::partial()      masks purrr::partial()
    ## ✖ readr::spec()       masks yardstick::spec()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors
    ## 
    ## Attaching package: 'gratia'
    ## 
    ## 
    ## The following object is masked from 'package:stringr':
    ## 
    ##     boundary
    ## 
    ## 
    ## The following object is masked from 'package:plotrix':
    ## 
    ##     dispersion
    ## 
    ## 
    ## The following object is masked from 'package:dials':
    ## 
    ##     penalty

# Exploratory Analysis

For datasets and initial exploration of the data structure, descriptive
statistics of continuous variables, correlation analysis, and various
visualization techniques were conducted.

Looking at , the distribution of is approximately normal, as seen in
<<<<<<< HEAD
Figure (fig:d1-log-antibody-hist) and Figure (fig:d1-log-antibody-qq).
High and low outliers can be observed in the Figure
@ref(fig:d1-log-antibody-box). Most covariates have weak or low
correlation with each other. There is a high positive correlation
=======
Figure @ref(fig:d1-log-antibody-hist) and Figure
@ref(fig:d1-log-antibody-qq). High and low outliers can be observed in
the Figure @ref(fig:d1-log-antibody-box). Most covariates have weak or
low correlation with each other. There is a high positive correlation
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee
between and ($\rho = 0.72$) and a moderate negative correlation between
and ($\rho = -0.50$). There is a mild negative correlation between and
($\rho = -0.23$), ($\rho = -0.17$), and ($\rho = -0.15$). There is a
mild positive correlation between and ($\rho = 0.10$). The correlation
between and ($\rho = -0.06$), ($\rho = -0.04$), and ($\rho = -0.01$) are
near zero, indicating no linear relationship. Linear relationships can
be seen in Figure @ref(fig:d1-log-antibody-lin).

Exploring , the distribution of is also approximately normal, as shown
<<<<<<< HEAD
Figure (fig:d2-log-antibody-hist) and Figure (fig:d2-log-antibody-qq).
High and low outliers are again visible in the Figure
(fig:d2-log-antibody-box). Most covariates exhibit weak or low
correlation with each other. There is a high positive correlation
=======
Figure @ref(fig:d2-log-antibody-hist) and Figure
@ref(fig:d2-log-antibody-qq). High and low outliers are again visible in
the Figure @ref(fig:d2-log-antibody-box). Most covariates exhibit weak
or low correlation with each other. There is a high positive correlation
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee
between and ($\rho = 0.72$) and a moderate negative correlation between
and ($\rho = -0.53$). There is a mild negative correlation between and
($\rho = -0.16$), ($\rho = -0.11$), and ($\rho = -0.08$). A mild
positive correlation exists between and ($\rho = 0.08$). The
correlations between and ($\rho = -0.01$), ($\rho = -0.00$), and
($\rho = -0.25$) are near zero or weak, again suggesting no strong
linear relationship. Linear relationships can be seen in Figure
<<<<<<< HEAD
(fig:d2-log-antibody-lin).
=======
@ref(fig:d2-log-antibody-lin).
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee

    ##   id age gender race smoking height weight  bmi diabetes hypertension SBP LDL
    ## 1  1  50      0    1       0  176.1   68.3 22.0        0            0 130  82
    ## 2  2  71      1    1       0  175.7   69.6 22.6        0            1 149 129
    ## 3  3  58      1    1       1  168.7   76.9 27.0        0            0 127 101
    ## 4  4  63      0    1       0  167.4   90.0 32.1        0            1 138  93
    ## 5  5  56      1    1       0  162.7   83.9 31.7        0            0 123  97
    ## 6  6  59      1    3       0  167.8   86.8 30.8        0            1 132 108
    ##   time log_antibody
    ## 1   76    10.647154
    ## 2   82     9.889049
    ## 3  168    10.900712
    ## 4  105     9.906258
    ## 5  193     9.563081
    ## 6  143     8.837763

    ## 'data.frame':    5000 obs. of  14 variables:
    ##  $ id          : int  1 2 3 4 5 6 7 8 9 10 ...
    ##  $ age         : num  50 71 58 63 56 59 67 62 60 64 ...
    ##  $ gender      : int  0 1 1 0 1 1 0 1 0 1 ...
    ##  $ race        : Factor w/ 4 levels "1","2","3","4": 1 1 1 1 1 3 4 1 4 1 ...
    ##  $ smoking     : Factor w/ 3 levels "0","1","2": 1 1 2 1 1 1 1 1 1 1 ...
    ##  $ height      : num  176 176 169 167 163 ...
    ##  $ weight      : num  68.3 69.6 76.9 90 83.9 86.8 91.4 87.7 85.7 76.6 ...
    ##  $ bmi         : num  22 22.6 27 32.1 31.7 30.8 29.7 28.1 29 31.5 ...
    ##  $ diabetes    : int  0 0 0 0 0 0 0 0 0 0 ...
    ##  $ hypertension: num  0 1 0 1 0 1 1 0 0 1 ...
    ##  $ SBP         : num  130 149 127 138 123 132 133 130 129 134 ...
    ##  $ LDL         : num  82 129 101 93 97 108 89 96 120 135 ...
    ##  $ time        : num  76 82 168 105 193 143 63 78 61 88 ...
    ##  $ log_antibody: num  10.65 9.89 10.9 9.91 9.56 ...

    ##        id            age            gender       race     smoking 
    ##  Min.   :   1   Min.   :44.00   Min.   :0.0000   1:3221   0:3010  
    ##  1st Qu.:1251   1st Qu.:57.00   1st Qu.:0.0000   2: 278   1:1504  
    ##  Median :2500   Median :60.00   Median :0.0000   3:1036   2: 486  
    ##  Mean   :2500   Mean   :59.97   Mean   :0.4854   4: 465           
    ##  3rd Qu.:3750   3rd Qu.:63.00   3rd Qu.:1.0000                    
    ##  Max.   :5000   Max.   :75.00   Max.   :1.0000                    
    ##      height          weight            bmi           diabetes     
    ##  Min.   :150.2   Min.   : 56.70   Min.   :18.20   Min.   :0.0000  
    ##  1st Qu.:166.1   1st Qu.: 75.40   1st Qu.:25.80   1st Qu.:0.0000  
    ##  Median :170.1   Median : 80.10   Median :27.60   Median :0.0000  
    ##  Mean   :170.1   Mean   : 80.11   Mean   :27.74   Mean   :0.1544  
    ##  3rd Qu.:174.2   3rd Qu.: 84.90   3rd Qu.:29.50   3rd Qu.:0.0000  
    ##  Max.   :192.9   Max.   :106.00   Max.   :38.80   Max.   :1.0000  
    ##   hypertension         SBP             LDL             time      
    ##  Min.   :0.0000   Min.   :101.0   Min.   : 43.0   Min.   : 30.0  
    ##  1st Qu.:0.0000   1st Qu.:124.0   1st Qu.: 96.0   1st Qu.: 76.0  
    ##  Median :0.0000   Median :130.0   Median :110.0   Median :106.0  
    ##  Mean   :0.4596   Mean   :129.9   Mean   :109.9   Mean   :108.9  
    ##  3rd Qu.:1.0000   3rd Qu.:135.0   3rd Qu.:124.0   3rd Qu.:138.0  
    ##  Max.   :1.0000   Max.   :155.0   Max.   :185.0   Max.   :270.0  
    ##   log_antibody   
    ##  Min.   : 7.765  
    ##  1st Qu.: 9.682  
    ##  Median :10.089  
    ##  Mean   :10.064  
    ##  3rd Qu.:10.478  
    ##  Max.   :11.961

    ## Warning: Expected 2 pieces. Additional pieces discarded in 6 rows [67, 68, 69, 70, 71,
    ## 72].

| Variable | Min | Q1 | Median | Mean | Q3 | Max |
|:---|---:|---:|---:|---:|---:|---:|
| id | 1.000000 | 1250.750000 | 2500.50000 | 2500.50000 | 3750.25000 | 5000.00000 |
| age | 44.000000 | 57.000000 | 60.00000 | 59.96840 | 63.00000 | 75.00000 |
| gender | 0.000000 | 0.000000 | 0.00000 | 0.48540 | 1.00000 | 1.00000 |
| height | 150.200000 | 166.100000 | 170.10000 | 170.12634 | 174.22500 | 192.90000 |
| weight | 56.700000 | 75.400000 | 80.10000 | 80.10908 | 84.90000 | 106.00000 |
| bmi | 18.200000 | 25.800000 | 27.60000 | 27.74040 | 29.50000 | 38.80000 |
| diabetes | 0.000000 | 0.000000 | 0.00000 | 0.15440 | 0.00000 | 1.00000 |
| hypertension | 0.000000 | 0.000000 | 0.00000 | 0.45960 | 1.00000 | 1.00000 |
| SBP | 101.000000 | 124.000000 | 130.00000 | 129.90040 | 135.00000 | 155.00000 |
| LDL | 43.000000 | 96.000000 | 110.00000 | 109.90860 | 124.00000 | 185.00000 |
| time | 30.000000 | 76.000000 | 106.00000 | 108.86260 | 138.00000 | 270.00000 |
| log | 7.765405 | 9.681635 | 10.08908 | 10.06434 | 10.47758 | 11.96137 |

Clean Summary Statistics for Numeric Variables

    ##           id          age       gender         race      smoking       height 
    ##            0            0            0            0            0            0 
    ##       weight          bmi     diabetes hypertension          SBP          LDL 
    ##            0            0            0            0            0            0 
    ##         time log_antibody 
    ##            0            0

    ## [1] 0

<figure>
<img src="DS2_Midterm_files/figure-gfm/d1-log-antibody-hist-1.png"
alt="Histogram of log_antibody levels for dat1" />
<figcaption aria-hidden="true">Histogram of log_antibody levels for
dat1</figcaption>
</figure>

<figure>
<img src="DS2_Midterm_files/figure-gfm/d1-log-antibody-qq-1.png"
alt="Q-Q plot of log_antibody levels for dat1" />
<figcaption aria-hidden="true">Q-Q plot of log_antibody levels for
dat1</figcaption>
</figure>

<figure>
<img src="DS2_Midterm_files/figure-gfm/d1-log-antibody-box-1.png"
alt="Boxplot of log_antibody levels for dat1" />
<figcaption aria-hidden="true">Boxplot of log_antibody levels for
dat1</figcaption>
</figure>

    ##       age            height          weight            bmi       
    ##  Min.   :44.00   Min.   :150.2   Min.   : 56.70   Min.   :18.20  
    ##  1st Qu.:57.00   1st Qu.:166.1   1st Qu.: 75.40   1st Qu.:25.80  
    ##  Median :60.00   Median :170.1   Median : 80.10   Median :27.60  
    ##  Mean   :59.97   Mean   :170.1   Mean   : 80.11   Mean   :27.74  
    ##  3rd Qu.:63.00   3rd Qu.:174.2   3rd Qu.: 84.90   3rd Qu.:29.50  
    ##  Max.   :75.00   Max.   :192.9   Max.   :106.00   Max.   :38.80  
    ##       SBP             LDL             time        log_antibody   
    ##  Min.   :101.0   Min.   : 43.0   Min.   : 30.0   Min.   : 7.765  
    ##  1st Qu.:124.0   1st Qu.: 96.0   1st Qu.: 76.0   1st Qu.: 9.682  
    ##  Median :130.0   Median :110.0   Median :106.0   Median :10.089  
    ##  Mean   :129.9   Mean   :109.9   Mean   :108.9   Mean   :10.064  
    ##  3rd Qu.:135.0   3rd Qu.:124.0   3rd Qu.:138.0   3rd Qu.:10.478  
    ##  Max.   :155.0   Max.   :185.0   Max.   :270.0   Max.   :11.961

    ##                       age       height       weight          bmi          SBP
    ## age           1.000000000 -0.006857166 -0.002514628  0.002260399  0.439919900
    ## height       -0.006857166  1.000000000  0.229695087 -0.500674819  0.004814655
    ## weight       -0.002514628  0.229695087  1.000000000  0.724847296 -0.008630173
    ## bmi           0.002260399 -0.500674819  0.724847296  1.000000000 -0.009403136
    ## SBP           0.439919900  0.004814655 -0.008630173 -0.009403136  1.000000000
    ## LDL           0.212258203  0.020783067 -0.004389010 -0.018657875  0.253413373
    ## time         -0.030417250  0.008117138  0.015388365  0.007231242 -0.029774788
    ## log_antibody -0.150554867  0.103646141 -0.165836431 -0.225877963 -0.061278877
    ##                      LDL         time log_antibody
    ## age           0.21225820 -0.030417250  -0.15055487
    ## height        0.02078307  0.008117138   0.10364614
    ## weight       -0.00438901  0.015388365  -0.16583643
    ## bmi          -0.01865787  0.007231242  -0.22587796
    ## SBP           0.25341337 -0.029774788  -0.06127888
    ## LDL           1.00000000 -0.011881322  -0.03576689
    ## time         -0.01188132  1.000000000  -0.01384286
    ## log_antibody -0.03576689 -0.013842856   1.00000000

    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'

<figure>
<img src="DS2_Midterm_files/figure-gfm/d1-log-antibody-lin-1.png"
alt="Linearity between log_antibody levels and covariates for dat1" />
<figcaption aria-hidden="true">Linearity between log_antibody levels and
covariates for dat1</figcaption>
</figure>

    ##        id age gender race smoking height weight  bmi diabetes hypertension SBP
    ## 5001 5001  58      0    4       1  176.4   86.4 27.7        0            0 130
    ## 5002 5002  62      0    1       1  167.5   82.4 29.4        1            0 123
    ## 5003 5003  71      0    4       0  179.3   79.2 24.6        1            1 145
    ## 5004 5004  59      1    1       0  170.0   81.0 28.0        0            0 123
    ## 5005 5005  69      1    1       0  166.5   74.8 27.0        1            1 150
    ## 5006 5006  56      0    1       0  167.6   74.8 26.6        0            0 121
    ##      LDL time log_antibody
    ## 5001 115  205     9.810890
    ## 5002 118  229     9.076660
    ## 5003 149  206    10.432296
    ## 5004 119  163     9.831918
    ## 5005 142  240     9.074990
    ## 5006 112  206    10.182070

    ## 'data.frame':    1000 obs. of  14 variables:
    ##  $ id          : int  5001 5002 5003 5004 5005 5006 5007 5008 5009 5010 ...
    ##  $ age         : num  58 62 71 59 69 56 65 61 62 68 ...
    ##  $ gender      : int  0 0 0 1 1 0 0 1 0 0 ...
    ##  $ race        : Factor w/ 4 levels "1","2","3","4": 4 1 4 1 1 1 1 1 1 4 ...
    ##  $ smoking     : Factor w/ 3 levels "0","1","2": 2 2 1 1 1 1 1 2 1 1 ...
    ##  $ height      : num  176 168 179 170 166 ...
    ##  $ weight      : num  86.4 82.4 79.2 81 74.8 74.8 69.2 81.3 82.1 74.4 ...
    ##  $ bmi         : num  27.7 29.4 24.6 28 27 26.6 22.4 27.4 30.7 26.7 ...
    ##  $ diabetes    : int  0 1 1 0 1 0 0 0 0 0 ...
    ##  $ hypertension: num  0 0 1 0 1 0 1 0 1 1 ...
    ##  $ SBP         : num  130 123 145 123 150 121 132 120 142 137 ...
    ##  $ LDL         : num  115 118 149 119 142 112 127 76 86 123 ...
    ##  $ time        : num  205 229 206 163 240 206 285 185 124 127 ...
    ##  $ log_antibody: num  9.81 9.08 10.43 9.83 9.07 ...

    ##        id            age            gender      race    smoking     height     
    ##  Min.   :5001   Min.   :46.00   Min.   :0.000   1:663   0:601   Min.   :149.4  
    ##  1st Qu.:5251   1st Qu.:57.00   1st Qu.:0.000   2: 55   1:296   1st Qu.:166.1  
    ##  Median :5500   Median :60.00   Median :0.000   3:199   2:103   Median :170.2  
    ##  Mean   :5500   Mean   :60.02   Mean   :0.491   4: 83           Mean   :170.2  
    ##  3rd Qu.:5750   3rd Qu.:63.00   3rd Qu.:1.000                   3rd Qu.:174.2  
    ##  Max.   :6000   Max.   :75.00   Max.   :1.000                   Max.   :190.6  
    ##      weight            bmi           diabetes      hypertension  
    ##  Min.   : 58.80   Min.   :19.80   Min.   :0.000   Min.   :0.000  
    ##  1st Qu.: 75.30   1st Qu.:25.80   1st Qu.:0.000   1st Qu.:0.000  
    ##  Median : 80.20   Median :27.60   Median :0.000   Median :0.000  
    ##  Mean   : 80.13   Mean   :27.72   Mean   :0.157   Mean   :0.456  
    ##  3rd Qu.: 84.40   3rd Qu.:29.60   3rd Qu.:0.000   3rd Qu.:1.000  
    ##  Max.   :101.60   Max.   :35.80   Max.   :1.000   Max.   :1.000  
    ##       SBP             LDL             time        log_antibody   
    ##  Min.   :106.0   Min.   : 46.0   Min.   : 61.0   Min.   : 8.048  
    ##  1st Qu.:124.0   1st Qu.: 96.0   1st Qu.:140.0   1st Qu.: 9.502  
    ##  Median :130.0   Median :112.0   Median :171.0   Median : 9.935  
    ##  Mean   :129.6   Mean   :110.2   Mean   :173.8   Mean   : 9.897  
    ##  3rd Qu.:135.0   3rd Qu.:124.0   3rd Qu.:205.0   3rd Qu.:10.315  
    ##  Max.   :156.0   Max.   :174.0   Max.   :330.0   Max.   :11.852

    ##           id          age       gender         race      smoking       height 
    ##            0            0            0            0            0            0 
    ##       weight          bmi     diabetes hypertension          SBP          LDL 
    ##            0            0            0            0            0            0 
    ##         time log_antibody 
    ##            0            0

    ## [1] 0

<figure>
<img src="DS2_Midterm_files/figure-gfm/d2-log-antibody-hist-1.png"
alt="Histogram of log_antibody levels for dat2" />
<figcaption aria-hidden="true">Histogram of log_antibody levels for
dat2</figcaption>
</figure>

<figure>
<img src="DS2_Midterm_files/figure-gfm/d2-log-antibody-qq-1.png"
alt="Q-Q plot of log_antibody levels for dat2" />
<figcaption aria-hidden="true">Q-Q plot of log_antibody levels for
dat2</figcaption>
</figure>

<figure>
<img src="DS2_Midterm_files/figure-gfm/d2-log-antibody-box-1.png"
alt="Boxplot of log_antibody levels for dat2" />
<figcaption aria-hidden="true">Boxplot of log_antibody levels for
dat2</figcaption>
</figure>

    ##       age            height          weight            bmi       
    ##  Min.   :46.00   Min.   :149.4   Min.   : 58.80   Min.   :19.80  
    ##  1st Qu.:57.00   1st Qu.:166.1   1st Qu.: 75.30   1st Qu.:25.80  
    ##  Median :60.00   Median :170.2   Median : 80.20   Median :27.60  
    ##  Mean   :60.02   Mean   :170.2   Mean   : 80.13   Mean   :27.72  
    ##  3rd Qu.:63.00   3rd Qu.:174.2   3rd Qu.: 84.40   3rd Qu.:29.60  
    ##  Max.   :75.00   Max.   :190.6   Max.   :101.60   Max.   :35.80  
    ##       SBP             LDL             time        log_antibody   
    ##  Min.   :106.0   Min.   : 46.0   Min.   : 61.0   Min.   : 8.048  
    ##  1st Qu.:124.0   1st Qu.: 96.0   1st Qu.:140.0   1st Qu.: 9.502  
    ##  Median :130.0   Median :112.0   Median :171.0   Median : 9.935  
    ##  Mean   :129.6   Mean   :110.2   Mean   :173.8   Mean   : 9.897  
    ##  3rd Qu.:135.0   3rd Qu.:124.0   3rd Qu.:205.0   3rd Qu.:10.315  
    ##  Max.   :156.0   Max.   :174.0   Max.   :330.0   Max.   :11.852

    ##                      age      height      weight           bmi         SBP
    ## age           1.00000000  0.01798237 -0.02463596 -0.0339202130  0.49930403
    ## height        0.01798237  1.00000000  0.20220998 -0.5253746729 -0.01003387
    ## weight       -0.02463596  0.20220998  1.00000000  0.7242445669 -0.07821894
    ## bmi          -0.03392021 -0.52537467  0.72424457  1.0000000000 -0.06139821
    ## SBP           0.49930403 -0.01003387 -0.07821894 -0.0613982094  1.00000000
    ## LDL           0.18675915 -0.02426887 -0.01989479 -0.0002632226  0.23895512
    ## time         -0.04239180  0.03177441 -0.04599080 -0.0616083609  0.01860855
    ## log_antibody -0.07581041  0.08390950 -0.11496483 -0.1638775639 -0.01002340
    ##                        LDL        time log_antibody
    ## age           0.1867591543 -0.04239180  -0.07581041
    ## height       -0.0242688747  0.03177441   0.08390950
    ## weight       -0.0198947855 -0.04599080  -0.11496483
    ## bmi          -0.0002632226 -0.06160836  -0.16387756
    ## SBP           0.2389551203  0.01860855  -0.01002340
    ## LDL           1.0000000000  0.04049703  -0.00186483
    ## time          0.0404970331  1.00000000  -0.24812211
    ## log_antibody -0.0018648302 -0.24812211   1.00000000

    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'
    ## `geom_smooth()` using formula = 'y ~ x'

<figure>
<img src="DS2_Midterm_files/figure-gfm/d2-log-antibody-lin-1.png"
alt="Linearity between log_antibody levels and covariates for dat2" />
<figcaption aria-hidden="true">Linearity between log_antibody levels and
covariates for dat2</figcaption>
</figure>

![](DS2_Midterm_files/figure-gfm/unnamed-chunk-13-1.png)<!-- -->![](DS2_Midterm_files/figure-gfm/unnamed-chunk-13-2.png)<!-- -->![](DS2_Midterm_files/figure-gfm/unnamed-chunk-13-3.png)<!-- -->

The exploration and evaluation of is used to help build a prediction
model specific ally using GAM to understand how demographic and clinical
factors influence antibody responses and how antibody levels change over
time following vaccination. Considering the researcher collects a new
and independent dataset, , we discover the correlation between and is
stronger than in and similarly has weak linear relationships with most
covariates. allows us to evaluate the robustness and generalizability of
our prediction model.

# Model Trainging

A Generalized Additive Model (GAM) was created to model log-transformed
antibody level. Predictors included age, gender, race, smoking, height,
weight, BMI, diabetes, hypertension, SBP, LDL, and time since
vaccination. To prepare the data for modeling, the model matrix, x, was
created using the outcome and all predictors listed above and extracted
the response variable, y. Given that race and smoking were categorical
variables with multiple categories, some re-coding was necessary to use
these variables in the model building. Therefore, race and smoking were
converted into factor variables with “White” being the reference group
for race and “Never” being the reference group for smoking.

The GAM models were then fitted. The first model, gam.m1, is a standard
linear model with no smoothing terms. The second model, gam.m2, uses
smoothing on age, bmi, SBP, LDL, and time since vaccination. There was
reason to believe these variables were non-linear, therefore the
smoothing allowed the variables to be used in the model. Finally, model
3, gam.m3, includes a tensor product to model the interaction between
height and weight.

The three GAM models were then compared using an ANOVA test that
provides the f-test; this was used to determine which model provides the
best fit. Cross-validation for GAM tuning was then conducted using a
10-fold cross-validation to tune to GAM model. The best hyperparameters
and the final fitted model were then retrieved. The same model training
procedure was used with the new, independent dataset, dat2.

| Model  | Resid. Df | Resid. Dev |       Df |   Deviance |        F |   Pr(\>F) |
|:-------|----------:|-----------:|---------:|-----------:|---------:|----------:|
| gam.m1 |  4984.000 |   1509.442 |       NA |         NA |       NA |        NA |
| gam.m2 |  4971.177 |   1380.053 | 12.82350 | 129.389611 | 36.37749 | 0.0000000 |
| gam.m3 |  4968.540 |   1378.818 |  2.63652 |   1.234568 |  1.68820 | 0.1738572 |

ANOVA Comparison of GAM Models (Dat1)

<figure>
<img src="DS2_Midterm_files/figure-gfm/gam2-gridplot-1.png"
alt="Smooth terms for GAM model (gam.m2)" />
<figcaption aria-hidden="true">Smooth terms for GAM model
(gam.m2)</figcaption>
</figure>

<figure>
<img src="DS2_Midterm_files/figure-gfm/vis-gam-1.png"
alt="Visualization of Model 3 (dat1)" />
<figcaption aria-hidden="true">Visualization of Model 3
(dat1)</figcaption>
</figure>

    ##   select method
    ## 2   TRUE GCV.Cp

    ## 
    ## Family: gaussian 
    ## Link function: identity 
    ## 
    ## Formula:
    ## .outcome ~ gender + diabetes + hypertension + smoking + race + 
    ##     s(age) + s(SBP) + s(LDL) + s(bmi) + s(time) + s(height) + 
    ##     s(weight)
    ## 
    ## Estimated degrees of freedom:
    ## 0.991 0.000 0.000 4.179 7.892 1.234 0.000 
    ##  total = 23.3 
    ## 
    ## GCV score: 0.2786734

![](DS2_Midterm_files/figure-gfm/unnamed-chunk-16-1.png)<!-- -->![](DS2_Midterm_files/figure-gfm/unnamed-chunk-16-2.png)<!-- -->![](DS2_Midterm_files/figure-gfm/unnamed-chunk-16-3.png)<!-- -->

| Model  | Resid. Df | Resid. Dev |       Df |  Deviance |         F |   Pr(\>F) |
|:-------|----------:|-----------:|---------:|----------:|----------:|----------:|
| gam.m1 |  984.0000 |   275.4546 |       NA |        NA |        NA |        NA |
| gam.m2 |  977.7820 |   268.5783 | 6.217997 | 6.8762407 | 4.0341782 | 0.0004416 |
| gam.m3 |  976.6323 |   268.2745 | 1.149679 | 0.3038207 | 0.9640406 | 0.3384056 |

ANOVA Comparison of GAM Models (Dat2)

Model 2 (gam.m2) was chosen to be the final model based on the
improvements it made upon Model 1 (gam.m1), (pval=\<0.001).

![](DS2_Midterm_files/figure-gfm/unnamed-chunk-18-1.png)<!-- -->

![](DS2_Midterm_files/figure-gfm/unnamed-chunk-19-1.png)<!-- -->

# Final Model Results

    ##   select method
    ## 2   TRUE GCV.Cp

    ## 
    ## Family: gaussian 
    ## Link function: identity 
    ## 
    ## Formula:
    ## .outcome ~ gender + diabetes + hypertension + smoking + race + 
    ##     s(age) + s(SBP) + s(LDL) + s(bmi) + s(time) + s(height) + 
    ##     s(weight)
    ## 
    ## Estimated degrees of freedom:
    ## 0.991 0.000 0.000 4.179 7.892 1.234 0.000 
    ##  total = 23.3 
    ## 
    ## GCV score: 0.2786734

    ## MSE: 0.3249953

<figure>
<img src="DS2_Midterm_files/figure-gfm/dx-plots-1.png"
alt="Diagnostic Plots for Prediction Model on dat2" />
<figcaption aria-hidden="true">Diagnostic Plots for Prediction Model on
dat2</figcaption>
</figure>

The prediction model’s robustness and generalizability is mostly
acceptable for . Prediction accuracy was determined by the mean squared
<<<<<<< HEAD
error (MSE) at 0.325 showing a low average on unseen data. The
prediction model shows model stability with generalized cross-validation
(GCV) score of 0.279. Looking at (fig:dx-plots) we evaluate Predicted vs
Actual log_antibody Levels, Residuals vs Predicted, and the Distribution
of Residuals. Predictions are mostly aligned with the observed values
especially in the 9.5-10.5 predicted range. There is mild
under-prediction below value 9, which indicates that the model may tend
to underestimate lower antibody levels but perform well in the 9.5-10.5
predicted range. The predicted vs residual plot shows residuals mostly
centered and near 0, suggesting that there is no significant bias in the
model’s predictions. Right-skewness can be observed in the predicted vs
residual plots, which could suggest some non-linearity. The distribution
of residuals looks approximately normal and does not have extreme
outliers or multi-modality.
=======
error (MSE) at 0.325 showing a low average on unseen data. prediction
model shows model stability with generalized cross-validation (GCV)
score of 0.279. The Looking at @ref(fig:dx-plots) we evaluate Predicted
vs Actual log_antibody Levels, Residuals vs Predicted, and the
Distribution of Residuals. Predictions are mostly aligned with the
observed values especially in the 9.5-10.5 predicted range. There is
mild under-prediction below value 9. The predicted vs residual plot
shows residuals mostly centered and near 0. Right-skewness can be
observed in the predicted vs residual plots, which could suggest some
non-linearity. The distribution of residuals looks approximately normal
and does not have extreme outliers or multi-modality.
>>>>>>> f5e371ff37c9e841cbcaba1343c15e0de86916ee
