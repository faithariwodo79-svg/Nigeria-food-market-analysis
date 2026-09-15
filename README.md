Nigeria Food Market Analysis

Project Overview

This project explores food price data collected across Nigerian markets between January 2016 and July 2026.

The goal of the project is to clean, validate, standardize, and prepare food market data for analysis while identifying important data-quality issues that could affect further analysis.

The project combines food price records with market and commodity information to create a cleaner analytical dataset.

Objectives

- Audit the food price datasets for data-quality issues.
- Check for missing values and duplicate records.
- Identify unmatched market and commodity IDs.
- Standardize price measurements into comparable units.
- Investigate the distribution of retail and wholesale price records.
- Combine the food price data with market and commodity information.
- Produce a cleaned dataset suitable for further exploratory analysis.

Datasets

The project uses three related datasets:

- Food Prices — contains food price observations recorded across markets.
- Markets — contains information about the markets referenced by the price data.
- Commodities — contains information about the commodities being tracked.

Data Audit

The initial food price dataset contained 75,053 records covering 68 unique markets and 41 commodities.

Key audit results:

Check| Result
Food price records| 75,053
Unique markets in price data| 68
Unique commodities| 41
Unmatched market IDs| 1
Unmatched commodity IDs| 0
Orphan observations identified| 53
Final analytical records| 64,893

The unmatched market ID was investigated before the affected observations were excluded from the final analytical dataset.

Data Cleaning

Several cleaning and validation steps were performed:

1. Checked the datasets for missing values and duplicate records.
2. Validated market and commodity IDs against their corresponding reference datasets.
3. Investigated unmatched market records.
4. Checked for non-positive price values.
5. Standardized price measurements.
6. Converted gram-based observations to kilograms where appropriate.
7. Separated kilogram and liquid-unit observations for analysis.
8. Merged the cleaned price data with market and commodity information.

After cleaning and standardization, the final analytical dataset contained 64,893 records.

Tools & Technologies

- Python
- Pandas
- Jupyter Notebook
- Microsoft Excel
- Git & GitHub

Project Structure

Nigeria-food-market-analysis/
│
├── 01_data_audit.ipynb
├── food_prices.csv
├── markets.csv
├── commodoties (5).csv
├── cleaned_food_prices.xlsx
├── README.md
└── .gitignore

Key Takeaways

The data audit showed that the dataset contains a large number of food price observations covering more than ten years.

The audit also identified an unmatched market ID affecting 53 observations. Rather than ignoring the issue, the records were investigated and excluded from the final analytical dataset so that the resulting data could be reliably linked to the available market information.

The cleaned dataset provides a foundation for further analysis of food prices across commodities, markets, locations, and time.

Next Steps

Future analysis can explore:

- Food price trends over time.
- Differences between markets.
- Retail versus wholesale prices.
- Commodity price patterns.
- Regional price differences.
- Changes in food prices across different periods.

Author

Faith Ariwodo

Junior Data Analyst | Cyber Security Student

This project was completed as part of my data analytics learning and portfolio development.