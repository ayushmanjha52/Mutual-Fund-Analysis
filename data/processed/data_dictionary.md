
# Data Dictionary - Mutual Fund Analysis Project

## Tables Created:

### 1. dim_fund (Dimension Table)
- amfi_code (Primary Key)
- scheme_name
- fund_house
- category
- risk_grade

### 2. fact_nav (Fact Table)
- amfi_code
- date
- nav

### 3. fact_transactions (Fact Table)
- investor_id
- transaction_date
- amfi_code
- transaction_type
- amount_inr

## Notes:
- Star Schema design used
- Only valid transactions (amount > 0) included
- NAV is forward-filled for non-trading days
