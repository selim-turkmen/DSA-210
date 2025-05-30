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

- Visualized distributions of IQ, protein, and fat consumption.
- Created scatter plots and histograms to explore bivariate relationships.
- Assessed the linearity and outliers between variables.

3. ### Hypothesis Testing

– Formulated and tested the following hypotheses for nutrient intake vs IQ:

- **H₀:** There is no linear correlation between nutrient intake (protein or fat) and IQ.  
- **H₁:** There is a linear correlation between nutrient intake (protein or fat) and IQ.

– Applied Pearson correlation and p-value calculations to assess the strength and significance of the relationships.

> *Note:* Pearson correlation tests only for linear relationships. While strong linear trends were observed visually, possible non-linear effects were considered out of scope for this stage.

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

As an example, I created scatter plots to visualize the relationship between protein and fat consumption and average IQ.  
The plots showed a generally positive trend: higher protein and fat intake levels were both associated with higher average IQ.  

To test these relationships, I conducted a Pearson correlation analysis with the following hypotheses:

- **H₀:** There is no linear correlation between nutrient intake (protein or fat) and IQ.  
- **H₁:** There is a linear correlation between nutrient intake (protein or fat) and IQ.

Since the Pearson correlation coefficients for both protein and fat were positive and statistically significant (p < 0.001),  
we rejected the null hypothesis and concluded that a meaningful linear correlation likely exists in both cases.

> *Note:* Pearson correlation only captures linear relationships; nonlinear patterns, if any, are not addressed in this analysis.

Additionally, a 3D regression plot helped visualize the combined effect of both nutrients.

## Conclusion

This analysis explored the relationship between national average IQ levels and macronutrient intake, focusing on daily per capita protein and fat consumption. Both nutrients demonstrated statistically significant and moderately strong positive linear correlations with IQ. Pearson correlation coefficients and multiple linear regression models consistently supported this relationship, without indicating a dominant effect from either nutrient.

While protein and fat exhibited slightly different effect sizes, both contributed meaningfully to the variance in IQ. Importantly, no claim was made regarding causality or superiority of one nutrient over the other. The findings suggest that overall dietary macronutrient availability may play a role in shaping cognitive performance at a national level.

Future work may involve expanding the model to include additional dietary factors (e.g., micronutrients, caloric intake), socioeconomic variables (e.g., education, GDP per capita), or machine learning methods to capture potential nonlinearities. Nonetheless, the current study provides a clear, interpretable foundation for understanding how basic nutrition metrics relate to cognitive capacity across countries.
