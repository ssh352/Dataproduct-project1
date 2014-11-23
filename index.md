---
title       : Presentation of Mid-Atlantic Wage Data Analysis Application 
subtitle    : Developing Data Products Course Project
author      : Yao Wang
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Intruduction

- [Mid-Atlantic Wage Data Analysis Application](https://yaowang-data-app1.shinyapps.io/project/) is used to analyse Mid-Atlantic wage data. 
- Mid-Atlantic data is got from ISLR package Wage dataset.
- Wage dataset are records of wage and other data for a group of 3000 workers in the Mid-Atlantic region from 2003 to 2009.  

```r
library(ISLR)
data(Wage)  
```
     
     
[Source: http://thedataweb.rm.census.gov/TheDataWeb](http://thedataweb.rm.census.gov/TheDataWeb)  

Data was manually assembled by Steve Miller, of Open BI (www.openbi.com), from the March 2011 Supplement to Current Population Survey data.  
  
[References: An Introduction to Statistical Learning with applications in R](www.StatLearning.com)  
Games, G., Witten, D., Hastie, T., and Tibshirani, R. (2013), Springer-Verlag, New York  

--- .class #id

## Summary of Wage

```
## $year
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##    2000    2000    2010    2010    2010    2010 
## 
## $education
##       1. < HS Grad         2. HS Grad    3. Some College 
##                268                971                650 
##    4. College Grad 5. Advanced Degree 
##                685                426 
## 
## $jobclass
##  1. Industrial 2. Information 
##           1544           1456 
## 
## $wage
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##    20.1    85.4   105.0   112.0   129.0   318.0
```
  
--- .class #id  
  
## Slide4    

--- .class #id   

## How to use M.A. Wage Data Analysis Application  
This application is analysing wage data relative to different year, job class and education.  
- Choose "Year", "Job class" and "Education" from sidebar and submit your choice.  
- The summary of the coresponding wage shows: the minimum, the 1st quantile, the median, the mean, the 3rd quantile and the maximum.    

```r
summary(Wage$wage)
```

```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##    20.1    85.4   105.0   112.0   129.0   318.0
```
- The histogram plot shows the distribution of the wage.  

```r
hist(Wage$wage, xlab = "wage", col='lightblue', main = "Wage")
```

--- .class #id   
 
  
## Screenshot  
[https://yaowang-data-app1.shinyapps.io/project/]
(https://yaowang-data-app1.shinyapps.io/project/)

<div style='text-align: center;'>
    <img height='500' src='fig1.png' />
</div>







