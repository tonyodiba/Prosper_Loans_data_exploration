# Prosper Loan Data Exploration
## by Anthony Odiba


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554484977406000), This [data dictionary](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000) explains the variables in the data set.


## Summary of Findings

*most Prosper borrowers come from California. 
I checked U.S.A's population distribution by state and the Prosper Borrower number by state mirrors that.
*When we remove two highest non relevant Occupation classifications, we see that Computer Programmer is the Highest and Student-Technical School is the least.
*The Income Bracket borrowing the most from Prosper are the $25,000-$49,000, followed closely $50,000-$74,000 Income Bracket. When grouped by Employment Status, people listed as Employed borrowed more and "Retired" borrowed least.
*We have a right skewed multi-modal distribution for the LoanOriginalAmount.A lot of the loans are between \$0 and $10,000, with several peaks at \$5,000, \$10,000, \$15,000 and also to a lesser degree at \$20,000, and \$25,000. Interestingly, there's a steep jump in frequency at these amounts rather than a smooth ramp up. This suggests that people are more likely to request for loan amounts that are multiples of \$5,000.

*Most of the borrowers have a debt-to-income ratio below 1.0, and the tail gets really small past that number. There is an outlier value near 10.
*Most borrowers have 0 current delinquencies.
*A lot of the loans are current and have no issues. To compare with the other loan status effictively use a log scale.

* The ratio of home owners to those who do not own homes is almost equal.

*A lot of the BorrowerAPR occurs at 0.35797.

* In the dataset, ‘CreditGrade’ has around 29,000 entries and ‘ProsperRating’ has a little more than 85,000. In comparison to overall count, there are less High rating scores post 2009 than there were in pre-2009.It may be because after the company restructured, they implemented a stricter rating system.

*Graph of Prosper Score vs LoanStatus shows that it has a left-skewed distribution for completed loan, which means completed loans have primarily good ratings. However, Prosper score distributed a bell-shaped in high risk loan. Compared to Prosper Rating with a left-skewed shape, it seems like Prosper Score presents a less ability to detect the high risk loans.

>From the plot of both ProsperScore and CcreditGrade vs LoanStatus(i.e Performing and NonPerforming Loans), I observed that Prosper Score was way more efficient at determining the performance of a loan than creditGrade was. This indicates that the risk management system at Prosper is efficient.

*BorrowerAPR seems to be positively correlated with DebtToIncomeRatio and negatively correlated with  AvailableBankCardCredit.
It seems that a higher available bank card credit will lower  your interest rate. I theorise that when a borrower has relatively low credit amount the probabilities of getting low and high interest rates are similar, but with a high available bank credit, an individual is more likely to get a lower interest rate.

*The LoanOriginal amount vs Income Range, when grouped by performing vs Non-Performing loans, I observe that the two categories where non-performing loans is higher than performing loans are in the \$0 income range and the non employed.



## Key Insights for Presentation

For the presentation, I focus on viriables that had an effect on the ProsperScore or CreditGrade.  I start by introducing distribution of prosper loans around the U.S.A then we see how much various groups access Prosper loans. We delve deeper by observing how DebtToIncomeRatio vs BorrowerAPR interact with respect to CreditGrade, we then observe how StatedMonthlyIncome interacts with LoanAmount with respect to ProsperScore. We conclude with the strongest observed relationship; BorrowerAPR Vs ProsperScore. 

An interesting addition is a Parallel plot showing interaction of 9 different variables.