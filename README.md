# LogiTest Presentation

part1: part1.ipynb

part2: part2.ipynb

## For full project data, refers to Full(with data) folder. 

### Part1 Observations: 

1. Columns a to i might represent sales or products that were sold and later returned, or revenue.
2. There are 3 unique regions: 'LATAM', 'Asia Pacific', and 'America'.
3. There are 1249 unique SKUs.
4. Columns e and i are all 0s.
5. There are data type issues.
6. For columns a, c, and f, these columns are right-skewed.

### Part1 Fixes:

1. Convert 'fiscal_week_end_date' to datetime format.
2. For skewed datasets, we can use normalization.
3. For columns e and i, need to confirm the meaning of the numerical values.

### Anomaly Detection:

1. Use statistical metrics like mean, median, and standard deviation to find outliers in numerical columns. Z-score or IQR (Interquartile Range) methods can be effective.
2. Plotting data can sometimes reveal outliers directly. Box plots and scatter plots are particularly useful for this.

