# Factors Affecting Borrower APR in Prosper Loans
## by Chris Eldredge


## Dataset
This data set contains 113,937 loans from Prosper. The dataset includes loan amount, borrower rate (or interest rate), current loan status, and many other features.

## Summary of Findings

- There's a strong negative correlation between ProsperScore and BorrowerAPR. That is to say, as ProsperScore increases, BorrowerAPR decreases. This correlation makes sense, as ProsperScore is likely used to determine what interest rate to charge a borrower.
- The CreditScoreRangeUpper also appears to show a strong correlation with BorrowerAPR. As credit score increases, BorrowerAPR decreases.
- LoanOriginalAmount also correlates with BorrowerAPR. In general, the lower the LoanOriginalAmount, the lower the BorrowerAPR.
- DelinquenciesLast7Years is less correlated with BorrowerAPR than I expected. However, since most borrowers had no delinquencies this isn't that surprising
- Term of the loan appears to be correlated with LoanOriginalAmount. Larger loan amounts tend to have longer loan terms, which also intuitively makes sense as the borrower would need more time to repay a larger loan
- There were loans that defaulted across all levels of ProsperScore, but mostly concentrated in the mid to lower scores, indicating these borrowers were paying a higher APR to compensate for the higher likelihood of default. This trend suggests the ProsperScore is correctly identifying riskier borrowers and offering them higher APR.
- Defaults appear to be most common among smaller loan amounts
- The borrowers that defaulted had lower credit scores, as well (CreditScoreRangeUpper)
- Looking at the Current loans, it appears the lowest BorrowerAPR isn't offered for the largest loans. I would have thought at least a few borrowers with a low risk profile would be offered the lowest BorrowerAPR for larger loans.

## Key Insights for Presentation

- One of the strongest correlations is between ProsperScore and BorrowerAPR. As ProsperScore increases, BorrowerAPR decreases. This correlation makes sense, as ProsperScore is likely used to determine what interest rate to offer a borrower.
- Looking at the Defaulted category, there were loans that defaulted across all levels of ProsperScore, but mostly concentrated in the mid to lower scores. This indicates most borrowers that defaulted were paying a higher APR, suggesting that Prosper is correctly identifying riskier borrowers.