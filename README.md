## Table of Contents
- [Installation](#install)
- [Problem statement](#statement)
- [About this File](#describe)
- [Analysis and Results](#results)
- [Licensing, Authors, and Acknowledgements](#acknowledge)

<a id='install'></a>
### Installation
1. Python 3.6 and latest from [here](https://www.python.org/downloads/)
2. Anaconda distribution of Python from [here](https://www.anaconda.com/blog/anaconda-distribution-2022-10#).

<a id='statement'></a>
# YULU PROJECT

> ## About Yulu
Yulu is India’s leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting.
Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and convenient!

## Problem Statement

Yulu has recently suffered considerable dips in its revenues. They have contracted a consulting company to understand the factors on which the demand for these shared electric cycles depends. Specifically, they want to understand the factors affecting the demand for these shared electric cycles in the Indian market.

### _How you can help here_?

The company wants to know:

Which variables are significant in predicting the demand for shared electric cycles in the Indian market?
How well those variables describe the electric cycle demands?

#### _Concepts Used_:

Bi-Variate Analysis 2-sample t-test: testing for difference across populations ANNOVA Chi-square

#### _How to begin_:

1. Import the dataset and do usual exploratory data analysis steps like checking the structure & characteristics of the dataset
2. Try establishing a relation between the dependent and independent variable (Dependent “Count” & Independent: Workingday, Weather, Season etc)
3. Select an appropriate test to check whether:

> 1. Working Day has effect on number of electric cycles rented
> 2. No. of cycles rented similar or different in different seasons
> 3. No. of cycles rented similar or different in different weather
> 4. Weather is dependent on season (check between 2 predictor variable)

4. Set up Null Hypothesis (H0) State the alternate hypothesis (H1) Check assumptions of the test (Normality, Equal Variance). You can check it using Histogram, Q-Q plot or statistical methods like levene’s test, Shapiro-wilk test (optional).
5. Please continue doing the analysis even If some assumptions fail (levene’s test or Shapiro-wilk test) but double check using visual analysis and report wherever necessary.
6. Set a significance level (alpha) Calculate test Statistics. Decision to accept or reject null hypothesis. Inference from the analysis

<a id='describe'></a>
## About this file

1. `datetime`: datetime
2. `season`: season (1: spring, 2: summer, 3: fall, 4: winter)
3. `holiday`: whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
4. `workingday`: if day is neither weekend nor holiday is 1, otherwise is 0.
5. `weather`: 1: Clear, Few clouds, partly cloudy, partly cloudy 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
6. `temp`: temperature in Celsius
7. `atemp`: feeling temperature in Celsius
8. `humidity`: humidity
9. `windspeed`: wind speed
10. `casual`: count of casual users
11. `registered`: count of registered users
12. `count`: count of total rental bikes including both casual and registered

<a id='results'></a>
### Analysis and Results
I analysed the data and made inferences based on the results obtained from ANOVA and Chisquare tests. The code and the results are in this jupyter notebook __Yulu_inferential_statistics_project.ipynb__.

<a id='acknowledge'></a>
### Licensing, Authors, Acknowledgements
The data used for this analysis is [here](https://www.kaggle.com/datasets/ranitsarkar01/yulu-bike-sharing-data)