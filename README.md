readme_content = """
# Online Loan Analysis - Investment Study

## Overview

This analysis provides insights into online loan data, focusing on several key metrics such as Return on Investment (ROI), loan defaults, number of loans issued based on employment status, state, loan purpose, and other relevant factors. The dataset contains **39,717 rows and 55 columns**, with various derived metrics and visualizations.

## Data Shape

- **Rows**: 39,717
- **Columns**: 55

## Tools and Libraries

This analysis is conducted using Python 3.x with the following packages:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

## Data Cleaning

After loading the data, several data cleaning tasks were performed:

- **Data Type Fixes**: Adjusted data types for certain columns for better processing.
- **Date Conversion**: Converted the following columns from string to date type:
-  - `int_rate`
- **Whitespace Removal**: Removed extra spaces from the `term` column values.
- **Missing Values**: Handled missing data by:
  - Dropping columns with more than 30% missing values.
  - Filling missing values in the `revol_util` column with the mean value, as the mean and median were close.

## Analysis on Number of Loans Issued

- **Loan Grades**: A, B, and C grades had the highest number of loans issued, while G grade had the least.
- **Sub-Grades**: Sub-grades A4 and B3 were the most common among the loans issued.
- **Interest Rates**: Loans in grades A, B, and C had lower interest rates, while grades E, F, and G had higher interest rates.
  - This could be because A, B, and C grade applicants are likely to have better credit scores and pose less risk.
- **Funded Amount**: Higher loan amounts were associated with grades A, B, C, and D, as these applicants generally have better credit scores.
- **Employment Status**: A majority of the borrowers have been employed for at least 10 years.

## Analysis on Loan Defaulters

- **High Risk Categories**: More loan defaults were observed among borrowers with `RENT` and `MORTGAGE` homeownership statuses.
- **Loan Purpose**: Default rates were higher for loans with purposes like:
  - `debt_consolidation`
  - `other`
  - `credit_card`
  - `small_business`

## Conclusion

- Of the settled loans, 83% were fully paid, while 14% were charged off.
- Borrowers with homeownership (i.e., those who own a house) and loan purposes like `debt_consolidation`, `credit_card`, and `small_business` showed lower risk.
- The majority of loans were from grades A, B, and C.
- There is an inverse relationship between interest rates and loan grades. Lower grades (E, F, G) have higher interest rates.
- A higher percentage of defaulters came from the `debt_consolidation`, `other`, `credit_card`, and `small_business` loan purposes, irrespective of loan grade.

## Inspiration

This repository serves as a comprehensive guide for beginners to understand the entire process of **Exploratory Data Analysis (EDA)**, including:

- **Data Cleaning**
- **Data Preprocessing**
- **Data Visualization**

It covers both **categorical** and **numerical** data analysis, providing a solid foundation for EDA tasks. Whether you're new to data analysis or looking to expand your skills, this project will help you understand and implement key concepts.

---

### How to Use This Repository

1. Clone the repository to your local machine.
2. Install the required Python packages: `pandas`, `numpy`, `matplotlib`, and `seaborn`.
3. Explore the Jupyter notebooks for detailed analysis and visualizations.
4. Use the insights and code as a reference for your own data exploration tasks.
