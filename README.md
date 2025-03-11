# Quantium-Data-Analysis-Project

## Project Overview
This project analyzes the impact of a retail trial by comparing a trial store (where the trial was conducted) with a control store (a similar store not part of the trial). The goal is to determine whether the trial had a statistically significant effect on key performance metrics such as total sales and number of customers. The analysis involves selecting the most suitable control store, scaling its performance to match the trial store's pre-trial data, and assessing the trial's impact using statistical methods like t-tests and confidence intervals.

## Data Files
- `QVI_data_cleaned(CSV).gz`: Preprocessed dataset with cleaned retail transaction data
- `QVI_purchase_behaviour.csv`: Customer purchase behavior metrics and patterns
- `QVI_transaction_data.csv`: Detailed transaction-level data from retail operations
- `DATA_PROVENANCE.md`: Documentation of data sources and transformation processes

## Analysis Notebooks
- `qvi-retail-data-analysis.ipynb`: Main analysis notebook containing comprehensive data examination
- `retail-market-trends-qvi-transaction-data.ipynb`: Focused analysis of market trends in transaction data

## Methodology
1. **Data Cleaning**: Preprocessing raw transaction data to ensure quality and consistency
2. **Exploratory Data Analysis**: Investigating patterns and relationships in the retail data
3. **Control Store Selection**: Using correlation and magnitude distance to identify similar control stores
4. **Performance Scaling**: Adjusting control store metrics to match the trial store's pre-trial performance
5. **Statistical Analysis**: Implementing t-tests and confidence intervals to validate results

## Key Features
- Control store matching algorithm based on sales correlation and customer count similarity
- Time-series analysis of pre-trial and trial period performance metrics
- Statistical validation framework to determine significance of observed differences
- Comprehensive data visualization of key performance indicators and trends

## Data Provenance
For detailed information about the data sources, collection methods, and transformations applied during preprocessing, please refer to the [Data Provenance documentation](DATA_PROVENANCE.md).

## Technologies Used
- Python (Pandas, NumPy)
- Data visualization (Matplotlib, Seaborn)
- Statistical analysis libraries
- Jupyter Notebook

## Results
The analysis successfully quantifies the impact of the retail trial on sales performance and customer counts, providing statistical evidence of the trial's effectiveness with confidence intervals.

## Future Enhancements
- Segment analysis by customer demographics
- Additional performance metrics evaluation
- Machine learning models for predictive insights

## Tags
- exploratory-data-analysis
- data-analysis-python
- business-analysis
- retail-sales-analysis-using-python