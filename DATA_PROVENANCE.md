# Data Provenance

This document describes the source of the data used in this project and the transformations applied during collection and preprocessing.

## Data Sources

The data used in this project comes from the Quantium Virtual Internship program's retail analytics module. It consists of:

1. **QVI_transaction_data.csv**: Contains customer transaction data for a chips category from a major retail chain.
   - Source: Quantium sample retail dataset
   - Time period: July 2018 - June 2019
   - Contains: Transaction dates, store numbers, customer IDs, product quantity, and sales amounts

2. **QVI_purchase_behaviour.csv**: Contains customer segmentation and demographic information.
   - Source: Quantium customer database
   - Contains: Customer IDs, lifestage segments, and premium customer classifications

3. **QVI_data_cleaned(CSV).gz**: Compressed version of the cleaned and preprocessed transaction data.
   - Derived from: QVI_transaction_data.csv after data cleaning operations

## Data Transformation Process

The following transformations were applied to the raw data:

1. **Data Cleaning**:
   - Removed duplicate transactions
   - Filtered out outliers (extremely high transaction values)
   - Standardized date formats
   - Handled missing values through appropriate imputation methods

2. **Feature Engineering**:
   - Created time-based features (day of week, month, etc.)
   - Calculated derived metrics such as average purchase value
   - Aggregated transaction data by store and time periods

3. **Data Integration**:
   - Merged transaction data with customer behavior data using customer IDs
   - Combined store performance metrics with trial information

## Data Quality Assurance

To ensure data quality and integrity:
- Data validation checks were performed to identify inconsistencies
- Outlier detection and treatment was applied
- Missing value analysis and appropriate handling strategies were implemented
- Data distributions were examined for normality and other statistical properties

## Data Usage Limitations

This data is intended for educational and analytical purposes only. The data has been anonymized and does not contain personally identifiable information. Store numbers and other identifying information have been encoded to protect business confidentiality.

## Data Processing Tools

The data processing and analysis were conducted using:
- Python (Pandas, NumPy)
- Jupyter Notebooks
- Statistical analysis libraries