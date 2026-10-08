# Methodology

## Project Overview

This project analyzes household spending patterns and financial pressure using four quarters of the U.S. Bureau of Labor Statistics (BLS) Consumer Expenditure Survey (CES) Interview Survey, Family-Level Interview (FMLI) data.

The primary research question is:

> How do household spending patterns and financial pressure differ across quarters and household characteristics?

The analysis was conducted in Microsoft Excel using data cleaning, descriptive statistics, PivotTables, calculated variables, and visualizations.

## Data Preparation

The four quarterly datasets were cleaned and combined for analysis.

The analysis uses quarterly expenditure variables (PQ) and annual family income (`FINCBTXM`). Blank and negative values were removed where appropriate, while legitimate zero expenditure values were retained.

Observations with nonpositive annual family income were excluded from financial-pressure calculations because income is used as the denominator of the burden measures.

The analysis uses `REGION` to examine geographic differences and does not use `DIVISION`.

## Derived Variables

### Food Spending

Total food spending was constructed by combining food-at-home and food-away-from-home expenditures:

`FOODPQ = FDHOMEPQ + FDAWAYPQ`

### Household Size Group

Households were grouped according to household size to allow spending and income comparisons across different household sizes.

### Age Group

Reference persons were grouped into age categories to examine differences in income and spending across age groups.

### Income Group

Households were grouped by income to compare spending patterns and financial pressure across different income levels.

## Housing Burden

Quarterly housing expenditures (`EHOUSNGP`) were compared with annual family income (`FINCBTXM`).

Because housing expenditure is measured for a quarter while income is annual, quarterly housing spending was annualized:

`Estimated Annual Housing Spending = EHOUSNGP`

The constructed housing burden measure is:

`Estimated Annual Housing Burden = EHOUSNGP / (FINCBTXM/4)`

This measure is an analytical estimate rather than an official BLS housing-cost-burden measure. It assumes that the observed quarter is representative of annual housing spending.

## Shelter Burden

A separate shelter burden measure was calculated using shelter expenditures (`ESHELTRP`) and annual family income:

`Shelter Burden = ESHELTRP / (FINCBTXM/4)`

Both housing-related measures were retained because they capture different aspects of household housing pressure.

## Exclusions for Financial Pressure Analysis

Nonpositive income observations were excluded from financial-pressure calculations.

Constructed burden values greater than 1 were excluded from the financial-pressure analysis. These observations were treated as extreme or non-interpretable values for the constructed ratio.

These exclusions were applied to the financial-pressure analysis rather than to the entire dataset.

## Quarterly Analysis

The project compares Q1, Q2, Q3, and Q4 across key income and expenditure measures.

Quarterly observations were treated as separate observations. The analysis does not assume that households observed in different quarters are the same households.

Quarter-to-quarter comparisons were based on quarter-level averages rather than attempting to track individual households across quarters.

## Analysis Methods

The project uses:

- Descriptive statistics
- PivotTables
- Average and median comparisons
- Demographic group comparisons
- Age-group analysis
- Spending category analysis
- Quarterly comparisons
- Quarter × demographic comparisons
- Housing burden analysis
- Data visualizations
- Dashboard development

## Dashboard

The final dashboard summarizes:

- Household overview
- Quarter comparisons
- Spending composition
- Household comparisons
- Financial pressure

## Limitations

The quarterly datasets represent separate observations, so the analysis should not be interpreted as a longitudinal study of the same households across Q1–Q4.

The annualized housing burden measure is a constructed estimate based on one quarter of housing spending and annual family income. It therefore should not be interpreted as an official BLS housing-cost-burden statistic.

The results describe patterns in the analyzed CES observations and should be interpreted within the limitations of the survey data and the analytical choices made in this project.
