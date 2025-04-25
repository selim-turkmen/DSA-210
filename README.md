# DSA-210 Proposal Report

## Project Overview

Hi, I am Mustafa Selim Türkmen, a 2nd year student from Sabancı University. This is my DSA 210 term project. In this project, I investigate the relationship between countries’ average IQ levels and their nutritional habits that specifically focuses on daily per capita protein and fat consumption. 

The primary aim is to analyze whether these two nutritional indicators are correlated with national intelligence scores using global data from 2019. By utilizing official datasets from the FAO (Food and Agriculture Organization) and the Global IQ Index, I conducted exploratory data analysis, hypothesis testing, and regression modeling.

Ultimately, this project seeks to uncover potential associations between diet quantity and cognitive development across nations.

## Motivation

This project blends my interest in data-driven analysis with a commitment to addressing social issues. The key motivations include:

- **Social Impact:** Exploring how dietary consumption quantity may relate to national intelligence levels could inspire future improvements in public health and nutrition programs.
- **Accessible Data:** Leveraging global datasets from trusted sources like the FAO and Global IQ Index enables a transparent and reproducible analysis.
- **Scientific Curiosity:** Investigating whether protein and fat consumption can be associated with differences in average IQ across countries.
- **Policy Relevance:** Providing data-driven insights that could guide policies aiming to improve nutrition and cognitive development outcomes.

## Objectives

1. **Explore Correlations:**
   Examine whether there is a statistical relationship between countries' average IQ scores and their per capita protein and fat consumption.
2. **Conduct Hypothesis Testing:**
  Test the significance of observed correlations using formal statistical methods.
3. **Develop Regression Models:**
  Use linear and multivariable regression techniques to model the relationship between nutritional intake and IQ levels.
4. **Apply Data Science Methodologies:**
  Employ data preprocessing, exploratory analysis, visualization, modeling, and machine learning to generate actionable insights.

## Dataset

This project utilizes publicly available global datasets to analyze the relationship between *average IQ levels** and n*utritional intake** across countries. Specifically, the focus is on **daily per capita protein and fat consumption**.

### Data Sources
The data has been compiled from the following reliable sources:

- **Global IQ Index (2019):** Provides average national IQ scores, compiled from various studies and made available via https://www.theworldranking.com/statistics/461/countries-by-iq-average-iq-bycountry/
- **FAO Food Balance Sheets (2019):** Contains comprehensive data on daily food consumption per capita by country, including macronutrient details such as protein and fat.
- 
### Data Categories and Content
To improve clarity and interpretability, the data has been categorized as follows:

- **IQ Data:**
  - Average IQ scores by country (2019)
  - No missing values for selected countries included in final analysis

- **Nutrition Data:**
  - Daily per capita protein intake (grams)
  - Daily per capita fat intake (grams)
  - Values standardized and matched to corresponding IQ entries

### Data Format and Structure 
Both datasets were provided in CSV format and processed using Python and some Python libraries. Countries with missing or unmatched entries were excluded to ensure consistency and reliability. The final merged dataset contains IQ, protein, and fat values for each country. All preprocessing steps — including renaming, matching, and handling of outliers — were documented to ensure reproducibility.


## Tools and Technologies
I utilized the following tools and technologies throughout this project for data cleaning, analysis, hypothesis testing, and visualization:

- **Python:** For data analysis, hypothesis testing, and model development.
- **Pandas:** For preprocessing, cleaning, merging, and transforming data.
- **Matplotlib and Seaborn:** For generating visualizations such as scatter plots, histograms, regression graphs, and 3D plots.
- **Scikit-learn:** For statistical modeling and preparing groundwork for future machine learning tasks such as multivariate regression and feature importance analysis.

## Analysis Plan
 
1. ### Data Preparation

- Imported and merged IQ and nutrition datasets into Pandas DataFrames.
- Filtered the data to retain only 2019 values and aligned country names.
- Removed or excluded rows with missing or inconsistent entries.

2. ### Exploratory Data Analysis

- Analyze trends in crime and economic indicators over time across different regions.
- Visualize distributions of crime types and economic factors.
- Identify correlations between key economic variables and crime rates.
- Assess regional disparities in crime based on economic conditions.

3. ### Hypothesis Testing

- Formulate and test hypotheses:
  - **H₀:** There is a correlation between fat and protein consumption quantities and IQ.
  - **Hᵢ:** There is no correlation between fat and protein consumption quantities and IQ.
- Applied Pearson correlation and p-value calculations.

4. ### Regression Modeling

- Performed simple linear regression for each nutrient separately.
- Built a multivariable regression model including both protein and fat as predictors.
- Visualized regression planes in 3D to illustrate the combined effect.

5. ### Visualization and Reporting

- Designed plots that highlight trends and correlations clearly.
- Summarized findings with visual aids and statistical summaries.
- Interpreted results in a way that is accessible to both technical and non-technical audiences.

6. ### Future Machine Learning Applications

- Prepare dataset structures for supervised learning (e.g., using IQ as target variable).
- Explore multiple regression models and regularization techniques (Ridge, Lasso).
- Evaluate model performance using MAE, R², and cross-validation.
- Investigate the use of feature importance rankings to determine dominant nutritional indicators.

## Example Analysis

As an example, I created scatter plots to visualize the relationship between protein and fat consumption and average IQ. The plots showed a generally positive trend, with higher protein intake associated with higher IQ levels. Fat consumption showed a weaker but still noticeable trend.

To test the relationship, I conducted a correlation analysis and used the following hypotheses:

- **H₀:** There is a correlation between fat and protein consumption quantities and IQ.
- **Hᵢ:** There is no correlation between fat and protein consumption quantities and IQ.

Since the results did not provide strong enough evidence to reject the null hypothesis, I concluded that a correlation likely exists, especially between protein intake and IQ.

Additionally, a 3D regression plot helped visualize the combined effect of both nutrients.

## Conclusion

This project explored whether there is a correlation between countries’ average IQ levels and their daily per capita consumption of protein and fat.

Key insights include:

- Is there a measurable relationship between countries’ **protein and fat consumption** and their **average IQ levels**?
- Which nutrient shows a stronger correlation with IQ: protein or fat?
- Can **simple regression models** help explain national differences in cognitive performance?
- What insights can be drawn to inform future research or health and education policies?

The findings indicate that protein consumption shows a statistically significant correlation with IQ, while fat consumption appears to have a weaker but noticeable link. This suggests that dietary habits may influence cognitive outcomes at a population level.

In the next phase, I will begin applying machine learning methods to predict IQ based on nutritional and socioeconomic features, aiming to reveal deeper patterns beyond traditional analysis.
