# Project 1: SAT and ACT SCORES

#### Overview: 
This project was My first foray into the world of data science. The dataset contains the SAT and ACT scores of the graduating class of 2017. The dataset was aquired from PrepScholar.com. This project highlights the following skills: data cleaning and exploratory data analysis (EDA), data visualizations, conducting a hypothesis test, and generating a 95% confidence interval.

#### Data cleaning and EDA
By running a few basic methods we can check our data types, look for null values, and check some basic statistics to see if anything looks out of place. Right away we can see that Participation is stored as an object. By stripping the "%" we can convert the values into a float64 so that we can run mathematical fuctions on the column. By looking at the minimum and maximum of all the columns, we can see that there are two improper inputs, one under SAT mathscores, and one under ACT science scores. With a little bit of algebra, we can put the correct values into Maryland's observations.

The participation rate for ACT shows negative skew whereas SAT shows positive skew distribution, explaining more students are participating ACT test over SAT. 

#### Hypothesis testing
Setting up to test the hypothesis that SAT participation is different than the ACT participation rates.

$H_0: \mu SAT Participation = \mu ACT Participation$ 

$H_A: \mu SAT Participation \neq \mu ACT Participation$

The T-test produces a p-value of 0.00024 which is less than /alpha. We can reject the null Hypothesis and we are 95% confidence intervals for SAT and ACT participation rates are in between -.3105 and 1.1066 for SAT and 0.0069 to 1.2981 for ACT.

#### Conclusion
The results of the hypothesis test show that participation rates are higher for the ACT. Even though the tests cover the same subject matter, it seems that more students are taking the ACT. In order to find out why this is the case, we need nore data such as availability, test price, and to see if certain states have contracts with either of the testing companies.



