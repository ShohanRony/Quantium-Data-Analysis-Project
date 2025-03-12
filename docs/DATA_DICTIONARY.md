# Data Dictionary

This document provides comprehensive information about the variables in the datasets used for this analysis.

## Transaction Data (QVI_transaction_data.csv)

| Variable | Description | Type | Example Values |
|----------|-------------|------|---------------|
| DATE | Date of transaction | Date (YYYY-MM-DD) | 2018-07-01 |
| STORE_NBR | Unique store identifier | Integer | 1, 2, 3, ... |
| LYLTY_CARD_NBR | Loyalty card number | Integer | 12345, 67890, ... |
| TXN_ID | Transaction identifier | Integer | 1, 2, 3, ... |
| PROD_NBR | Product identifier | Integer | 1, 2, 3, ... |
| PROD_NAME | Product name/description | String | "Dorito Corn Chip 380g", "Smith Chip Thinly S/Cream 175g", ... |
| PROD_QTY | Quantity of product purchased | Integer | 1, 2, 3, ... |
| TOT_SALES | Total sales amount | Float | 5.00, 7.50, ... |

## Customer Data (QVI_purchase_behaviour.csv)

| Variable | Description | Type | Example Values |
|----------|-------------|------|---------------|
| LYLTY_CARD_NBR | Loyalty card number | Integer | 12345, 67890, ... |
| LIFESTAGE | Customer life stage segment | String | "YOUNG SINGLES/COUPLES", "OLDER SINGLES/COUPLES", "NEW FAMILIES", ... |
| PREMIUM_CUSTOMER | Premium customer classification | String | "Premium", "Mainstream", "Budget" |

## Cleaned Data (QVI_data_cleaned(CSV).gz)

This is a compressed version of the cleaned and joined dataset containing:

| Variable | Description | Type | Example Values |
|----------|-------------|------|---------------|
| DATE | Date of transaction | Date (YYYY-MM-DD) | 2018-07-01 |
| STORE_NBR | Unique store identifier | Integer | 1, 2, 3, ... |
| LYLTY_CARD_NBR | Loyalty card number | Integer | 12345, 67890, ... |
| TXN_ID | Transaction identifier | Integer | 1, 2, 3, ... |
| PROD_NBR | Product identifier | Integer | 1, 2, 3, ... |
| PROD_NAME | Product name/description | String | "Dorito Corn Chip 380g", "Smith Chip Thinly S/Cream 175g", ... |
| PROD_QTY | Quantity of product purchased | Integer | 1, 2, 3, ... |
| TOT_SALES | Total sales amount | Float | 5.00, 7.50, ... |
| LIFESTAGE | Customer life stage segment | String | "YOUNG SINGLES/COUPLES", "OLDER SINGLES/COUPLES", "NEW FAMILIES", ... |
| PREMIUM_CUSTOMER | Premium customer classification | String | "Premium", "Mainstream", "Budget" |
| PACK_SIZE | Package size extracted from product name | String | "380g", "175g", ... |
| BRAND | Brand name extracted from product name | String | "Dorito", "Smith", ... |
| CATEGORY | Product category | String | "CORN CHIP", "POTATO CHIP", ... |

## Derived Metrics Used in Analysis

| Metric | Description | Calculation |
|--------|-------------|-------------|
| Total Sales | Sum of sales for a given store and time period | SUM(TOT_SALES) |
| Total Customers | Count of unique customers | COUNT(DISTINCT LYLTY_CARD_NBR) |
| Average Sales per Customer | Average sales amount per customer | Total Sales / Total Customers |
| Sales Index | Normalized sales measure for comparison | (Store Sales / Baseline Sales) * 100 |
| Customer Count Index | Normalized customer count for comparison | (Store Customer Count / Baseline Customer Count) * 100 |
| Correlation Coefficient | Measure of sales pattern similarity between stores | Pearson correlation between time series |
| Magnitude Distance | Measure of absolute difference in sales volumes | SQRT(SUM((Store1 Sales - Store2 Sales)²)) |
| T-statistic | Statistical measure for hypothesis testing | (Observed Difference - 0) / Standard Error |
| P-value | Probability of observing results by chance | Derived from t-statistic and degrees of freedom |
| Confidence Interval | Range of values that likely contains the true effect | Point Estimate ± (Critical Value * Standard Error) |