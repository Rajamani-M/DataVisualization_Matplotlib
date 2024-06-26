# Pymaceuticals, Inc.: Study of Anti-Cancer Medications

## Overview

Pymaceuticals, Inc. conducted a study to screen potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. In this study, 249 mice identified with SCC tumors received treatment with various drug regimens over 45 days. The objective was to evaluate the effectiveness of Pymaceuticals’ drug of interest, Capomulin, against other treatment regimens. This repository includes the analysis of the study data, with detailed visualizations and statistical summaries.

## Repository Structure

- `data/`: Contains the study data files.
  - `Mouse_metadata.csv`: Metadata about the mice used in the study.
  - `Study_results.csv`: Results of the study.
- `Pymaceuticals_analysis.ipynb`: Jupyter Notebook containing the analysis, visualizations, and summary statistics.
- `README.md`: This file, providing an overview and instructions for the project.

## Instructions

### Prepare the Data

1. **Merge the Data**: Combine `Mouse_metadata` and `Study_results` DataFrames.
2. **Check for Duplicates**: Identify any duplicate entries based on `Mouse ID` and `Timepoint`.
3. **Clean the Data**: Remove duplicate entries to ensure the data is clean.

### Generate Summary Statistics

Calculate the following summary statistics for each drug regimen:

- Mean Tumor Volume
- Median Tumor Volume
- Tumor Volume Variance
- Tumor Volume Standard Deviation
- Tumor Volume Standard Error of the Mean (SEM)

### Create Bar Charts and Pie Charts

- **Bar Charts**: Show the total number of timepoints for all mice tested for each drug regimen.
  - One bar chart using Pandas.
  - One bar chart using Matplotlib's pyplot.
  
- **Pie Charts**: Show the distribution of female versus male mice in the study.
  - One pie chart using Pandas.
  - One pie chart using Matplotlib's pyplot.

### Calculate Quartiles, Find Outliers, and Create a Box Plot

1. **Final Tumor Volume**: Determine the final tumor volume for each mouse across four treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
2. **Quartiles and Outliers**: Calculate the quartiles, IQR, and identify any potential outliers for these treatments.
3. **Box Plot**: Generate a box plot to show the distribution of the final tumor volume for each treatment group.

### Create a Line Plot and a Scatter Plot

1. **Line Plot**: Plot tumor volume vs. time point for a single mouse treated with Capomulin.
2. **Scatter Plot**: Plot mouse weight vs. average observed tumor volume for the entire Capomulin regimen.

### Calculate Correlation and Regression

1. **Correlation Coefficient**: Calculate the correlation between mouse weight and average tumor volume for the Capomulin regimen.
2. **Linear Regression Model**: Fit a linear regression model and plot it on the scatter plot.

## Observations

1. **Effectiveness of Capomulin and Ramicane**: Both Capomulin and Ramicane significantly reduced tumor volumes compared to other treatments, with fewer outliers indicating consistent results.
2. **Tumor Volume Distribution**: The box plot analysis shows that Capomulin and Ramicane had the lowest median tumor volumes and fewer potential outliers.
3. **Correlation Between Weight and Tumor Volume**: A positive correlation exists between mouse weight and average tumor volume in the Capomulin regimen, suggesting heavier mice tend to have larger tumors.

## Hints and Bonus

- **Hints**:
  - Use the provided code comments in the Jupyter Notebook to guide you through each step of the analysis.
  - Refer to Stack Overflow and the Matplotlib documentation for additional guidance on plotting and data manipulation.
  
- **Bonus**:
  - Explore additional visualizations to further understand the data, such as histograms of tumor volumes or heatmaps of correlations between different variables.
  - Perform a more detailed statistical analysis to compare the effectiveness of the drug regimens.

## How to Run the Notebook

1. Ensure you have Python and Jupyter Notebook installed.
2. Clone this repository.
3. Navigate to the repository directory.
4. Launch Jupyter Notebook by running `jupyter notebook` in your terminal.
5. Open `Pymaceuticals_analysis.ipynb` and run the cells sequentially to reproduce the analysis and visualizations.

## Conclusion
This analysis provides insights into the effectiveness of different treatment regimens in reducing tumor volumes in mice with SCC. The visualizations and statistical summaries highlight the potential of Capomulin and Ramicane as effective treatments, guiding further research and development.

