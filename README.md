# Retail Analytics: Quantium Data Analysis Project

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.4.2-green.svg)
![NumPy](https://img.shields.io/badge/NumPy-1.22.4-yellow.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5.2-red.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📊 Project Overview

This data analysis project evaluates the effectiveness of a retail trial by comparing performance metrics between trial and control stores. Using statistical methods and data visualization techniques, the analysis determines whether the trial resulted in significant improvements in sales and customer engagement.

### Business Problem

A retail client implemented a trial of new layouts and product placements in select stores. The key business questions were:
- Did the trial generate a statistically significant uplift in sales?
- Did the trial attract more customers to the stores?
- Should the changes be rolled out to all stores in the network?

## 🔍 Key Features

- **Control Store Selection Algorithm**: Developed a robust methodology for identifying comparable control stores using correlation and magnitude distance metrics
- **Time Series Analysis**: Implemented time-based analysis of pre-trial and trial period performance
- **Statistical Validation**: Applied t-tests and confidence intervals to validate findings
- **Data Visualization**: Created comprehensive visualizations to communicate complex patterns and insights
- **Business Recommendations**: Translated analytical findings into actionable business strategies

## 📂 Repository Structure

```
├── data/                   # Data directory
│   ├── QVI_transaction_data.csv         # Raw transaction data
│   ├── QVI_purchase_behaviour.csv       # Customer segmentation data
│   └── QVI_data_cleaned(CSV).gz         # Cleaned and processed data
│
├── notebooks/              # Jupyter notebooks
│   ├── qvi-retail-data-analysis.ipynb           # Main analysis notebook
│   └── retail-market-trends-qvi-transaction-data.ipynb  # Market trends analysis
│
├── docs/                   # Documentation
│   ├── EXECUTIVE_SUMMARY.md             # Business-focused summary of findings
│   ├── DATA_DICTIONARY.md               # Detailed variable descriptions
│   ├── BUSINESS_RECOMMENDATIONS.md      # Actionable recommendations
│   └── DATA_PROVENANCE.md               # Data source information
│
├── .gitignore              # Git ignore file
├── requirements.txt        # Project dependencies
└── README.md               # Project overview (this file)
```

## 🧮 Methodology

The analysis followed a structured approach:

1. **Data Preparation & Cleaning**
   - Processed transaction and customer data
   - Extracted product attributes from descriptions
   - Created time-based features for trend analysis

2. **Exploratory Data Analysis**
   - Examined sales patterns and customer behavior
   - Identified seasonal trends and product preferences
   - Analyzed customer segments and purchasing habits

3. **Control Store Selection**
   - Developed metrics to measure store similarity
   - Selected optimal control stores based on pre-trial performance
   - Validated selection through correlation analysis

4. **Performance Assessment**
   - Scaled control store data to match trial store baseline
   - Measured performance during trial period
   - Calculated percentage differences in key metrics

5. **Statistical Testing**
   - Implemented hypothesis testing framework
   - Calculated confidence intervals for observed differences
   - Determined statistical significance of results

## 📈 Key Findings

- **Sales Performance**: Trial stores showed statistically significant sales uplift compared to control stores
- **Customer Engagement**: Increase in both customer count and average transaction value
- **Category Impact**: Premium products and family-size packages showed strongest response
- **ROI Analysis**: Projected positive return on investment for chain-wide implementation

For a detailed executive summary of findings, see the [Executive Summary](docs/EXECUTIVE_SUMMARY.md).

## 💼 Business Impact

The analysis provided clear evidence that the trial changes should be implemented across the store network, with an estimated positive ROI. Specific recommendations include:

- Phased rollout strategy prioritizing stores with similar demographics
- Enhanced merchandising for high-performing product segments
- Targeted marketing approach based on customer segment response

For complete business recommendations, see the [Business Recommendations](docs/BUSINESS_RECOMMENDATIONS.md) document.

## 🛠️ Technologies Used

- **Python**: Primary programming language
- **Pandas & NumPy**: Data manipulation and numerical analysis
- **Matplotlib & Seaborn**: Data visualization
- **SciPy & StatsModels**: Statistical testing and modeling
- **Jupyter Notebook**: Development environment

## 📚 Documentation

- [Data Dictionary](docs/DATA_DICTIONARY.md): Comprehensive description of all variables
- [Data Provenance](docs/DATA_PROVENANCE.md): Information about data sources and transformations
- [Executive Summary](docs/EXECUTIVE_SUMMARY.md): Business-focused overview of findings
- [Business Recommendations](docs/BUSINESS_RECOMMENDATIONS.md): Actionable insights and strategies

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Required packages listed in requirements.txt

### Installation
```bash
# Clone this repository
git clone https://github.com/ShohanRony/Quantium-Data-Analysis-Project.git

# Navigate to project directory
cd Quantium-Data-Analysis-Project

# Install dependencies
pip install -r requirements.txt

# Open Jupyter notebooks
jupyter notebook
```

## 👤 About Me

I'm Shohinur Pervez Shohan, a data analyst with strong skills in Python, statistical analysis, and business intelligence. This project demonstrates my ability to:

- Process and analyze large retail datasets
- Apply statistical methods to business problems
- Develop data-driven recommendations
- Communicate complex findings clearly

I'm currently seeking data analysis opportunities. Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/shohinur-pervez-shohan/) or via email at shohinur.pervez.shohan@gmail.com.

## 📄 License

This project is available for review and educational purposes. The data has been anonymized to protect business confidentiality.

## 🏷️ Tags
`data-analysis` `python` `retail-analytics` `statistical-testing` `business-intelligence` `exploratory-data-analysis` `time-series-analysis` `hypothesis-testing` `customer-segmentation`