# Real Estate EDA
Simple exploratory data analysis of a real estate dataset.  
This project contains a short, practical notebook that inspects data quality, missing values, summary statistics, correlations and the price distribution.
## Dataset
- File: `real_estate_dataset.csv`  
- Contains property records including `Price` and other features (numerical and categorical).
## What I did
- Load and inspect the data (head, shape, dtypes).
- Clean column names and handle missing values (median for numeric, `"missing"` for categorical).
- Basic statistics and `describe()`.
- Visual analysis: missing values (missingno), histogram + KDE, boxplot, correlation heatmap.
- Short interpretation of the price distribution and recommendations.
## Key findings
- Price distribution is unimodal with a slight right skew — a few expensive properties pull up the mean.
- Boxplot shows a wide spread and at least one clear high-price outlier.
- Median is a better measure of a “typical” property price in this dataset.
- Suggested next steps: log-transform target (or cap outliers), feature engineering, baseline models.
## How to run
1. Put `real_estate_dataset.csv` in the repository root.
2. Open `real_estate_eda.ipynb` in Jupyter or Colab.
3. Run cells from top to bottom.
(If you prefer Colab upload, the notebook contains a fallback cell to upload the CSV manually.)
## Requirements
- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- missingno

