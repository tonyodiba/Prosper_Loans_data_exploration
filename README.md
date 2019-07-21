[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tonyodiba/Prosper_Loans_data_exploration.git/master)

# Prosper Loan Data Exploration
## by Anthony Odiba


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554484977406000), This [data dictionary](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000) explains the variables in the data set.
***
## Note: 
**The files are too large for github to render so please note important instructions below**
> - [x] 1. Click this [link](https://mybinder.org/v2/gh/tonyodiba/Prosper_Loans_data_exploration.git/master) if you didn't notice binder badge above
> - [x] 2. Alternatively if you like doing things the harder way use [html preview](https://htmlpreview.github.io/) to view them.
   > > * To do 2 above, simply copy the link to the file you want to view, paste in the url bar provided on the page
> - [x] 3. My final .ipynb was too large(~64MB), obviously too large to upload to github so i used [Git Large File Storage](https://git-lfs.github.com/). The instructions on how to do this can be seen on the site.
> - [ ] I think there are some ways to reduce the file size by dropping some columns of the dataset used. I haven't explored this.
***
## Visualisation Libraries Used
Apart from the usual suspects, i.e seaborn, matplot, etc, I played around with **folium, plotly and plotly express** to come up with some beautiful and useful visualisations for this project.

## Summary of Findings

* Check [the Prosper loan Exploration file](https://github.com/tonyodiba/Prosper_Loans_data_exploration/blob/master/ProsperLoan_exploration_readme.md) for the summary findings.

## Key Insights for Presentation

For the presentation, I focus on viriables that had an effect on the ProsperScore or CreditGrade.  I start by introducing distribution of prosper loans around the U.S.A then we see how much various groups access Prosper loans. We delve deeper by observing how DebtToIncomeRatio vs BorrowerAPR interact with respect to CreditGrade, we then observe how StatedMonthlyIncome interacts with LoanAmount with respect to ProsperScore. We conclude with the strongest observed relationship; BorrowerAPR Vs ProsperScore. 

An interesting addition is a Parallel plot showing interaction of 9 different variables.

