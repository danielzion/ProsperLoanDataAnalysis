# (Dataset Exploration Title)
## by OLANIYAN Daniel Olusegun


## Preliminary Wrangling

This project is divided into two major sections

> In the first, an exploratory data analysis of a dataset was conducted. Python programming and data visualization libraries was used to explore the dataset's variables and understand the data's structure, pattern's and relationships.

> This analysis is structured as the Univariate, Bi-variate and Multivariate relationship was investigated.

> In the second, findings from our exploration was taken and then conveyed through exploratory analysis. A slide deck was created to communicate findings easily.


## Dataset

> This document explores a dataset containing borrower's APR and attributes for approximately 113,937 Prosper Loan Data with 80 features (ListingKey, Term, BorrowerAPR, BorrowerRate, LenderYield, EstimatedEffectiveYield, EstimatedLoss, EstimatedReturn, ProsperRating (numeric), ProsperScore, IsBorrowerHomeowner, CreditScoreRangeLower, CreditScoreRangeUpper, etc). Most variables are numeric in nature, but the variables Term, Loan_Status,IsBorrowerHomeowner are some of the categorical factor variables. While factors CurrentCreditLines, OpenCreditLines, OpenRevolvingAccounts are also a few of the ordered factors.

>In this project only 16 features will be explore out of the 80 features.

> Since our main goal here is EDA , I decided to merge the data assessment and cleaning steps into one to make it explicit and I left the code here by choice for future referencing and more understanding of the original and cleaned datasets.


## Data Assessing and Cleaning

> 1. Select important data columns features to visualize
> 2. Rename the selected columns to a uniform naming casing
> 3.  Check for null values 
> 4. Drop null values if they exist
> 5. Drop duplicated rows using the listing key as the Unique Identifier 


## Summary of Findings

> I'm most interested in figuring out what features are best for predicting the borrower's Annual Percentage Rate (APR) for the loan and how  loan terms, Prosper Rating associates with various metrics in the dataset.

> The Borrowers with the largest APR all have a 36 months term, with loan status predominantly completed or Chargedoff with an exemption of a single defaulted.

> the borrower APR decreases with the better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR. Borrowers with better prosper rating also have lower estimated losses, estimated effective yields and lower borrower rate.

> Most borrowers chose to go for loans with term of 36, while less borrowers chose the 60 term loans while very few borrowers chose the 12months term loan

>There is a interaction between categorical term and Prosper rating features. Proportionally, there are more 60 month loans on B and C ratings. There is only 36 months loans for HR rating borrowers. For loan amount, there is a interaction between term and rating.

> The distribution of APR looks multimodal. A small peak centered at 0.09, a large peak centered at 0.18. There is also a small peak centered 0.29. Additionally, there is a very sharp peak between 0.35 and 0.36. Only very few loans have APR greater than 0.41.

## Key Insights for Presentation

> The figure shows that the borrower APR decreases with the better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR. Borrowers with better prosper rating also have lower estimated losses, estimated effective yields and lower borrower rate.

> For the presentation, I only focused on features that could affect the borrower APR, which are loan Status, Prosper rating, loan terms, estimated return and estimated loss. I started by showing the distribution of borrower APR and loan status. Then, I showed the relationship between APR, borrower Rate, estimated effective yield, estimated return and estimated loss. I also investigated the effect of rating on relationship between APR and estimated return, as well as the effect of rating on relationship between borrower APR and term.