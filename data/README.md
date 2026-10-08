# Data

## Source

This project uses quarterly data from the U.S. Bureau of Labor Statistics (BLS) Consumer Expenditure Survey (CES) Interview Survey, Family-Level Interview (FMLI) files.

## Quarterly Data

The analysis uses four quarterly datasets:

- Q1
- Q2
- Q3
- Q4

The quarterly files were cleaned and combined for analysis in Microsoft Excel.

## Data Handling

The original quarterly datasets were not included in this repository. The GitHub repository contains the completed analysis rather than the full raw survey files.

Each quarterly observation is treated as a separate observation. The analysis does not assume that the same household appears in every quarter.

## Variables

Key variables used in the analysis include:

- `NEWID` — Consumer unit identifier
- `FINLWT21` — Final survey weight
- `AGE_REF` — Age of reference person
- `FAM_SIZE` — Family size
- `EDUC_REF` — Education of reference person
- `CUTENURE` — Housing tenure
- `REGION` — Census region
- `FINCBTXM` — Annual family income
- `ETOTALP` — Total expenditures
- `EHOUSNGP` — Housing expenditures
- `ETRANPTP` — Transportation expenditures
- `HEALTHPQ` — Healthcare expenditures

Additional expenditure and demographic variables are documented in the project's data dictionary.
