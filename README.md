# -Employee-Data-Analysis-Using-Python-Key-Findings-and-Trends-
This analysis delves into a dataset containing employee information such as Employee Position ,Age  ,Salary, Team. Using Python, we have identified prominent trends in workforce demographics, salary distributions, and correlations between variables. 

## Description
The analysis focuses on:
 - Distribution of employees across teams and positions. 
 - Predominant age groups within the workforce.
 - Insights into salary expenditure by team and position. 
 - Correlation between age and salary, represented visually.

## Steps

### Data Preprocessing and cleaning
1.The dataset had 9 columns which included Name,Position,Team,Salary,College Name,Height,Weight and Number.Among these 'Height' column had error values fully in string format.
As part of the requirement, we generated random values between 150cm and 180cm(Usual height range in human) using randint function of random module.
2.Having the look at the null values in the dataset columnwise using '.ismull()'function, it was found around 2% values in 'Salary' and around 18% values in 'College' are null.Since the college name is not significantly required for our analysis, we have replced null values with 'Not Provided'.For teh missing salary values, we have replced it with salary median whcih is the positional average.

### Analysis

#### 1.Team Distribution Analysis: Percentage split of employees across teams.

