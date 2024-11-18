# -Employee-Data-Analysis-Using-Python-Key-Findings-and-Trends-
### This analysis delves into a dataset containing employee information such as Employee Position ,Age  ,Salary, Team. Using Python, we have identified prominent trends in workforce demographics, salary distributions, and correlations between variables. 

## Description
### The analysis focuses on:
 ### - Distribution of employees across teams and positions. 
 ### - Predominant age groups within the workforce.
 ### - Insights into salary expenditure by team and position. 
 ### - Correlation between age and salary, represented visually.

## Steps

### Data Preprocessing and cleaning
#### 1.The dataset had 9 columns which included Name,Position,Team,Salary,College Name,Height,Weight and Number.Among these 'Height' column had error values fully in string format.As part of the requirement, we generated random values between 150cm and 180cm(Usual height range in human) using randint function of random module.
#### 2.Having the look at the null values in the dataset columnwise using '.ismull()'function, it was found around 2% values in 'Salary' and around 18% values in 'College' are null.Since the college name is not significantly required for our analysis, we have replced null values with 'Not Provided'.For teh missing salary values, we have replced it with salary median whcih is the positional average.

### Analysis

#### 1.Team Distribution Analysis: Percentage split of employees across teams.
##### Using the bar plot function of the seaborn library we plotted the teamwise distribution of the employees. We have inferred that there are 30 teams with highest employee count(4.15%) in teams ‘New Orleans Pelicans’. Most of the teams have same employee ratio which is 3.28%.

#### 2.Position Categorization: Segregation of employees by roles.
##### Out of 458 employees,22.3% which amounts to a count of 102 are in ‘SG’ position whereas only 17.2 % are in ‘C’ position.We can infer that employee ratio in each position is almost same and there is no much variability.We have plotted the representation using pie plot of mathplotlib library.

#### 3.Predominant Age Group: Identifies the age group with the highest representation.
##### For determining the age predominant age group in employees, we have plotted using histogram.From the histogram, we can infer that most of employees belong to the age group between 25-30.After the age of 30,there is a significant decrease in the number of employees hired by the company.

#### 4.Salary Insights: Determines which teams and positions account for the highest salary expenditure.
##### First we used the groupby function plot the salary expenditure teamwise and positionwise and tehn we used bar chart to plot this data for the top 5. It is understood that SF position from the team "Los Angeles Lakers" has the highest salary expenditure followed by the PF position from team "Miami Heat".Among the top 5 , we can see SF postion from team "Denver Nuggets" in 5th position.This is the inference when we anlayse the salary expenditure teamwise put in together with position.But, when we analyse the salary expenditure separately for Position and team, we can see that position 'C' has the highest salary expenditure and teamwise team 'Cleveland Cavaliers' has the highest salary expenditure.

#### 5.Correlation Analysis: Examines the relationship between age and salary.
##### We have used scatter plot function to plot the correlation between salary and age.There does not appear a strong correlation between the Age and Salary, although salary seems to slightly increase with the age for some individuals. This trend is inconsistent.Among the same age group(30-35), there is high variability in the salaries of the employees implying that attributes other than age like job position ,company and experience contribute to their high/low salaries.Most of the individuals draw salary below 10M irrespective of their age.





