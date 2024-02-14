Pymaceuticals Inc. Mouse Study Analysis

Project Overview:

This project involves the analysis of a mouse study conducted by Pymaceuticals Inc. The study explores the effects of various drug regimens on tumor growth in mice. The analysis includes data cleaning, statistical summaries, visualization of key findings, and interpretation of the results.

Project Structure:

The project consists of the following files:

* analysis.ipynb: Jupyter Notebook containing the Python code for the analysis.
* data/Mouse_metadata.csv: CSV file containing metadata about the mice used in the study.
* data/Study_results.csv: CSV file containing the results of the study, including measurements and observations.

Dependencies:

- Matplotlib
- Pandas
- Scipy

Key Findings:

- Data Cleaning:

- Duplicate mouse data was identified and removed.

- The final clean dataset contains information on 249 mice.

Summary Statistics:

- Mean, median, variance, standard deviation, and SEM of tumor volume were calculated for each drug regimen.

- The summary_stat DataFrame provides a concise overview of tumor volume characteristics for each drug regimen.
  We can use this information to compare the effectiveness of different treatments.

Bar and Pie Charts:

- Bar charts show the total number of mice for each drug regimen.
- Both Pandas and Pyplot plots serve the same purpose: visualizing the distribution of mice across different drug regimens.
- The Pandas plot is created directly from the mice_count data, while the Pyplot plot is manually constructed using extracted data.

- In the first pie chart: The line of code calculates the count of each unique value in the "Sex" column.
Specifically, it counts how many mice are labeled as male and how many are labeled as female.
The resulting pie chart shows the proportion of female and male mice in the dataset.

- The second pie charts depict the distribution of male and female mice in the study. 

Quartiles, Outliers, and Boxplots:

* Summary Statistics and Outliers:

- The snippet iterates through a list of drug names (Capomulin, Ramicane, Infubinol, Ceftamin).

For each drug, it calculates the following:

Quartiles: Lower quartile (25th percentile), median (50th percentile), and upper quartile (75th percentile) of tumor volume.

Interquartile Range (IQR): The difference between the upper and lower quartiles.

Potential Outliers: Values below the lower bound (Q1 - 1.5 * IQR) or above the upper bound (Q3 + 1.5 * IQR).

Specific Results:

* For Capomulin:

Lower quartile: 32.38
Upper quartile: 40.16
IQR: 7.78
Potential outliers: Values below 20.71 or above 51.83.

* For Ramicane:

Lower quartile: 31.56
Upper quartile: 40.66
IQR: 9.1
Potential outliers: Values below 17.91 or above 54.31.

* For Infubinol:

Lower quartile: 54.05
Upper quartile: 65.53
IQR: 11.48
Potential outliers: Values below 36.83 or above 82.75.

* For Ceftamin:

Lower quartile: 48.72
Upper quartile: 64.3
IQR: 15.58
Potential outliers: Values below 25.35 or above 87.67.

Observations:

- The snippet provides insights into the distribution of tumor volumes for different drug regimens.
- It highlights potential outliers that may require further investigation.


Box Plot Interpretation:

* Capomulin and Ramicane:

- These two regimens have similar median tumor volumes, which suggests they might be more effective in reducing tumor size.

- The boxes for Capomulin and Ramicane are relatively small, indicating less variability in tumor volumes within these groups.

- The whiskers extend to a reasonable range, capturing most of the data points.

* Infubinol:

- The median tumor volume for Infubinol is higher than that of Capomulin and Ramicane.

- The box is wider, indicating greater variability in tumor volumes within this group.

- There is an outlier in the Infubinol group, where one mouse has a significantly lower tumor volume compared to the rest.

* Ceftamin:

- Ceftamin also has a higher median tumor volume.

- The box is similar in width to Infubinol, suggesting variability in tumor volumes.

- No outliers are visible in the Ceftamin group.

Overall Insights:

- Capomulin and Ramicane appear promising due to their lower median tumor volumes.

- Infubinol has a wider range of tumor volumes, and the outlier may need further investigation.

- Ceftamin’s performance is comparable to Infubinol but lacks outliers.

Line and Scatter Plots:

Line plot displays the tumor volume over time for a selected mouse on the Capomulin regimen. The line connecting the data points illustrates the overall trend in tumor volume over the observed time points. We can observe inconsistent trend where the line slopes upward suggesting an increase in tumor volume over time, indicating potential tumor growth. Conversely, the line slopes downward, suggesting a decrease in tumor volume, indicating a potential response to treatment.

Scatter plot shows the relationship between mouse weight and average tumor volume for the Capomulin regimen. It shows a strong relationship between mouse weight and average tumor volume for the Capomulin regimen.
Correlation and Regression:

Correlation coefficient and linear regression model were calculated for mouse weight and average tumor volume in the Capomulin regimen.
A correlation coefficient of 0.83 indicates a strong positive linear relationship between two variables. The magnitude (0.83) suggests a strong positive correlation, indicating that as mouse weight increases, the average observed tumor volume tends to increase by approximately 83% of the change in the first variable.

