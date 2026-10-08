# Household Spending & Financial Pressure

## Overview

This project analyzes household spending patterns and financial pressure using data from the U.S. Bureau of Labor Statistics (BLS) Consumer Expenditure Survey (CES) Interview Survey.

The analysis examines how household income, spending, household characteristics, and housing costs vary across quarters and demographic groups.

## Research Question

> How do household spending patterns and financial pressure differ across quarters and household characteristics?

## Objectives

- Examine household income and expenditure patterns.
- Compare spending across quarters.
- Analyze spending differences across household characteristics.
- Examine the relationship between housing spending and household income.
- Identify differences in financial pressure across income groups and quarters.

## Dataset

**Source:** U.S. Bureau of Labor Statistics (BLS) Consumer Expenditure Survey (CES) Interview Survey

The project uses quarterly Family-Level Interview (FMLI) data for four quarters.

The analysis combines the quarterly datasets while treating each quarterly observation as a separate observation rather than assuming that the same household appears in every quarter.

## Tools

- Microsoft Excel
- PivotTables
- Excel formulas
- Data cleaning and validation
- Data visualization

## Key Variables

### Household Characteristics
- Household size
- Age of reference person
- Education
- Sex
- Region
- Housing tenure
- Income group

### Income
- Annual family income (`FINCBTXM`)

### Expenditures
- Total expenditures (`ETOTALP`)
- Housing (`EHOUSNGP`)
- Food at home and away from home
- Transportation (`ETRANPTP`)
- Healthcare (`HEALTHPQ`)
- Apparel (`APPARPQ`)
- Entertainment (`EENTRMTP`)
- Education (`EDUCAPQ`)
- Personal care (`PERSCAPQ`)
- Reading (`READPQ`)
- Tobacco (`TOBACCPQ`)
- Personal insurance (`PERINSPQ`)
- Miscellaneous (`EMISCELP`)

## Analysis

The Excel workbook contains the following sections:

- Raw Data
- Cleaned Data
- Data Dictionary
- Data Quality
- Descriptive Statistics
- Demographic Analysis
- Age Analysis
- Category Analysis
- Quarter Analysis
- Quarter × Demographic Analysis
- Financial Pressure Analysis
- PivotTables
- Visualizations
- Dashboard
- Findings

### Financial Pressure

Two housing-related measures are examined:

**Broad Housing Pressure**

Housing spending relative to annual family income.

**Shelter Burden**

Shelter spending relative to annual family income.

Quarterly housing spending is annualized when constructing the housing burden measure to align it with annual family income.

## Dashboard

The final Excel dashboard summarizes:

- Household overview
- Quarter comparisons
- Spending composition
- Household comparisons
- Financial pressure

## Key Skills Demonstrated

- Data cleaning
- Data validation
- Excel formulas
- PivotTables
- Descriptive statistics
- Demographic analysis
- Quarterly analysis
- Financial pressure analysis
- Data visualization
- Dashboard development
- Analytical interpretation

## Limitations

The quarterly CES observations are analyzed as separate observations. The analysis does not assume that observations from different quarters represent the same household.

The housing burden measure is a constructed estimate based on quarterly housing spending and annual family income. It should therefore be interpreted as an analytical measure rather than an official BLS housing-cost-burden measure.

Current quarter expenditures have limited amount of data, so previous quarter expenditures were used. It works out because the data files for the calendar year start with the second quarter and end with the first quarter of the next year.

## Files

- `Household_Spending_Financial_Pressure.xlsx` — Complete Excel analysis and dashboard
- `methodology.md` — Methodology and analytical decisions
- `findings.md` — Summary of findings
- `data_dictionary.xlsx` — Variable definitions and descriptions
