# DSA-210 Proposal Report

## Project Overview

Hi, I am Mustafa Selim Türkmen, a 2nd year student from Sabanci University. This is my DSA 210 term project. In this project, I will explore the relationship between crime rates and economic conditions across various cities in the United States. My primary aim is to examine how economic situations—such as unemployment rates, median household income, and education levels—correlate with different types of crime (e.g., violent crimes, theft, and property crimes). To achieve this, I will merge crime data from reliable sources like the FBI Crime Data Explorer with socioeconomic data from the United States Census Bureau and the Bureau of Labor Statistics. Ultimately, I aim to uncover meaningful patterns and insights that can inform better social policies and community safety initiatives.

## Motivation

This project blends my interest in data-driven analysis with a commitment to addressing social issues. The key motivations include:

- **Social Impact:** Understanding the link between economic factors and crime can lead to improved policies and safer communities.
- **Practical Data Access:** Comprehensive datasets from sources like the FBI and U.S. Census Bureau make this analysis feasible.
- **Scientific Curiosity:** Investigating the extent to which economic conditions are correlated with crime rates.
- **Policy Implications:** Providing insights that can assist policymakers in designing effective interventions.

## Objectives

1. **Identify Correlations:**
   Explore the relationships between crime rates (e.g., violent and property crimes) and economic indicators (e.g., unemployment, income, poverty, education).
2. **Determine Critical Factors:**
  Identify which economic variables have the most significant impact on different types of crime.
3. **Develop Predictive Models:**
  Utilize machine learning techniques to predict crime rates based on economic conditions.
4. **Apply Data Science Methodologies:**
  Employ data preprocessing, exploratory analysis, visualization, modeling, and machine learning to generate actionable insights.

## Dataset

This project uses multiple publicly available datasets to analyze the relationship between crime rates and economic indicators across various U.S. regions. The data includes crime statistics, socioeconomic indicators, labor market data, and demographic factors.

### Data Sources
The data has been gathered from the following reliable open data sources:

- **FBI Crime Data Explorer:** Annual and state-level crime statistics.
- **United States Census Bureau:** Demographic and income distribution data.
- **Bureau of Labor Statistics (BLS):** Unemployment rates, average income levels, and employment trends.
- **County Health Rankings & Roadmaps:** Regional health, social welfare, and economic disparity indicators.

### Data Categories and Content
Due to the large volume of variables spanning different formats and years, the datasets have been categorized for better interpretability:

- **Crime Data:**
  - Crime rates by city and state
  - Types of crimes (e.g., homicide, assault, theft)
  - Annual crime trends

- **Economic Indicators:**
  - Median household income and income distribution
  - Poverty rates and income inequality
  - Unemployment rates and sectoral employment levels

- **Demographic and Social Factors:**
  - Education levels (high school and college graduation rates)
  - Population density, age distribution, and ethnic composition
  - Regional health and social welfare statistics

###Data Format and Structure 
The datasets are in CSV and JSON formats, so they work with analysis tools. Since there are tens of thousands of records and hundreds of variables, unnecessary or missing data has been removed. The most important variables were chosen for analysis. The datasets were also combined at the state and county levels to make comparisons and find connections. This helps to understand how crime rates relate to economic and social factors, leading to useful insights and better policies.


## Tools and Technologies
I'll utilize the following tools and technologies throughout this project for comprehensive data analysis and visualization:

- **Python:** For statistical analysis, data manipulation, and machine learning.
- **Pandas:** For data cleaning, preprocessing, and merging.
- **Matplotlib and Seaborn:** For creating visualizations such as scatter plots, heatmaps, bar charts, and time series graphs.
- **Scikit-learn:** For developing predictive models (e.g., regression analysis and feature selection).

## Analysis Plan
 
1. ### Data Preparation

- Import and merge crime and economic data into Pandas DataFrames.
- Clean the data by handling missing values and standardizing units.
- Convert date fields to appropriate datetime formats.

2. ### Exploratory Data Analysis

- Analyze trends in crime and economic indicators over time across different regions.
- Visualize distributions of crime types and economic factors.
- Identify correlations between key economic variables and crime rates.
- Assess regional disparities in crime based on economic conditions.

3. ### Hypothesis Testing

- Formulate and test hypotheses:
  - **H₀:** Economic factors have no significant impact on crime rates.
  - **Hᵢ:** At least one economic factor significantly affects crime rates.
- Use regression analysis to identify the strongest predictors.

4. ### Predictive Modeling

- Develop machine learning models to predict crime rates based on economic conditions.
- Apply regression models (e.g., linear regression, random forest regression) to understand key relationships.
- Evaluate model performance using appropriate metrics.

5. ### Trend Analysis and Forecasting

- Examine patterns in crime trends over time.
- Analyze the impact of economic fluctuations on crime.
- Forecast future crime rates using statistical methods based on economic data.

6 .### Visualization and Reporting

- Create detailed visualizations such as scatter plots, heatmaps, and time series graphs.
- Summarize key findings and insights in a structured report.
- Provide actionable recommendations for policymakers.

## Example Analysis

I will make a scatter plot to show the connection between unemployment and crime rates. The x-axis will display the unemployment rate in a city, and the y-axis will show the total crime rate per person. If the points form an upward trend, it could mean that higher unemployment is linked to more crime.
Another example is studying income inequality and crime rates. By comparing areas with large income gaps to those with more equal incomes, I can see if economic inequality leads to higher crime rates.
I will also look at crime trends over time during economic ups and downs. If crime rates rise during recessions, it could suggest a link between financial struggles and increased crime.


## Conclusion

By the end of this project, I aim to answer the following key questions:

- Which economic indicators have the strongest correlation with crime rates?
- How do unemployment rates and income inequality influence various types of crime?
- Can predictive modeling effectively forecast crime trends based on economic data?
- What insights can be drawn to inform policy decisions and improve crime prevention strategies?

This analysis will contribute to a deeper understanding of crime patterns and support data-driven decisions in public policy and law enforcement. By comprehending the impact of economic conditions on crime, we can work toward more effective social programs and interventions.

