## Vehicle Records Inventory: Exploratory Data Analysis Report

## Project Objective
This project aims to explore and summarize a vehicle records dataset using exploratory data analysis techniques. The analysis focuses on understanding the dataset's 
characteristics, evaluating data quality, examining the distribution of key vehicle attributes, identifying trends and relationships among variables, and presenting 
findings through appropriate statistical summaries and visualizations.

## Key Technical Insights & Findings

1. Univariate Baseline
- Uniform Distributions: Continuous variables ('Mileage') and discrete variables ('Year') exhibit uniform distributions across the entire dataset. 
- Data Bounds: Production years span uniformly from 2000 to 2025, while odometer readings are evenly distributed between 10,000 and 300,000 miles.

2. Analytical Proof of Feature Independence
- Decoupled Age & Wear: Cross-examination of 'Year' vs. 'Mileage' yields perfectly straight, parallel vertical data columns with a completely horizontal regression line.
  Odometer readings are unaffected by vehicle age.
- Balanced Categorical Profiles: Grouped aggregations reveal that the 8 vehicle brands split evenly down the middle by chronological generation (4 brands possess a median
  year of 2012, while the other 4 possess a median year of 2013).
- Identical Category Metrics: The mean, median, and standard deviation for mileage profiles remain structurally identical across all discrete splits, including 'Fuel Type'
  and 'Transmission'. 

3. Data Quality Diagnosis
   The absolute geometric uniformity and complete absence of cross-categorical correlation across the 5,000 records serve as a strong diagnostic signal
   that this dataset functions as a synthetically generated or randomized matrix rather than organic real-world market data.

## Environment Setup & Tools
- Language: Python
- Libraries: 'pandas', 'matplotlib', 'seaborn'
- Global Visual Configuration:
  python
  sns.set_theme(style = "whitegrid")
  plt.rcParams['figure.figsize'] = (9, 3.5)
