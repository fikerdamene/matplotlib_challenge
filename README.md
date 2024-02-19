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

- The final clean dataset contains information on 248 mice.

Summary Statistics:

- Mean, median, variance, standard deviation, and SEM of tumor volume were calculated for each drug regimen.

- The summary_stat DataFrame provides a concise overview of tumor volume characteristics for each drug regimen.
  We can use this information to compare the effectiveness of different treatments.

Bar and Pie Charts:

- Bar charts show the total number of mice for each drug regimen.
- Both Pandas and Pyplot plots serve the same purpose: visualizing the distribution of mice across different drug regimens.
- The Pandas plot is created directly from the mice_count data, while the Pyplot plot is manually constructed using extracted data.

Bar and Pie Charts
Bar plots are generated using both Pandas and Matplotlib's pyplot to display the total number of rows (Mouse ID/Timepoints) for each drug regimen. Pie charts are generated to visualize the distribution of female versus male mice in the cleaned dataset using both Pandas and Matplotlib.


Quartiles, Outliers, and Boxplots
The final tumor volume for each mouse across specific treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin) is calculated. Quartiles, potential outliers, and boxplots are generated to visualize the distribution of final tumor volumes for each treatment regimen.


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

