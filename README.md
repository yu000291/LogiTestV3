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

### Part2: 

1. How would you join the two data structures (sales data and product line data) to setup the analysis?

All SKUs in df_dt are in df_pl and all SKUs in df_pl are in df_dt, just use basic left join. 

2. What is the year over year growth by month of the product lines?

See part2.ipynb.

3. What methods/charts would you use to visualize the sales?

Heatmap, Stacked Bar Chart, Line Chart.
  
4. What inferences can be made from the data?

Growth Trends: mix of positive and negative growth rates.

Seasonality: "Karax- Rainbow" has consistently high growth rates in the second half of the year (September to December).

Variability: "Recoil" and "Stalker" show high variability.

Consistency: "WCB-Barcelona" and "WCB-Rangoon Nara" show relatively consistent growth rates.

Overall, positive trend over time.

  
5. How would you tier store level performance using a function?

Tier 1 to 5, percentile thresholds : [-6.259, 19.028, 62.312, 116.242]

1 means the highest performance, 5 means the lowest.

6. Warehouse assignment

    
See part2.ipynb.
