# Investment-Study: Online Loan Analysis

## Overview
This report explores trends and insights from online loan data, focusing on metrics like Return on Investment (ROI), loan defaults, and borrower profiles.

## Data Details
- **Rows**: 39,717
- **Columns**: 111
- **Tools**: Python 3.0, pandas, numpy, matplotlib, seaborn

## Methods Used
1. Data Cleaning:
   - Fixed column values and data types.
   - Imputed missing values using mean.
   - Dropped columns with >70% missing values.
2. Data Analysis:
   - Trends in loan grades, interest rates, and employment.
   - Risk analysis for defaulters based on loan purpose and housing.

## Key Findings
- **Loan Trends**:
  - Majority of loans are from A, B, and C grades.
  - Inverse relationship between loan grade and interest rate.
- **Defaulters**:
  - Most defaulters rent or mortgage their homes.
  - Loan purposes like 'debt_consolidation' and 'credit_card' have higher default rates.
### Conclusion

1. **Loan Status:**
   - Of the settled loans, 83% were fully paid, while 14% were charged off.

2. **Borrower Risk Profile:**
   - Borrowers owning houses and those with loans for purposes like debt consolidation, credit card repayment, and small businesses are generally lower risk.  
   - In contrast, borrowers who rent or have mortgages pose a higher default risk.

3. **Loan Grades:**
   - The majority of loans fall under A, B, and C grades.  
   - Lower-grade loans (E, F, G) correspond to higher interest rates, indicating an inverse relationship between interest rate and loan grade.

4. **Profitability Insights:**
   - Borrowers with top-tier credit profiles or smaller loan amounts do not necessarily yield the highest ROI.  
   - Borrowers with lower credit grades (E, F, G) proved to be more profitable despite their higher risk.

5. **Default Trends:**
   - Across all grades, the highest default rates were observed in loans taken for debt consolidation, other purposes, credit card repayment, and small businesses.

## Inspiration
This analysis serves as a comprehensive guide for beginners in data exploration, covering cleaning, preprocessing, and visualization techniques.

## Acknowledgment
Do fork and upvote this repository if you find it useful!
