# Marriage & Divorce Data Analysis (EDA)

## Introduction
Welcome to the **Marriage & Divorce Data Analysis** repository! In this project, we explore marriage and divorce trends in **Iran💚🤍❤️** using publicly available data from kaggle. Our goal is to gain insights into these significant life events and understand how they have evolved over time.

## Table of Contents

1. Introduction
2. Data Sources
3. Exploratory Data Analysis
4. Key Findings
5. Methodology
6. Code Samples
7. Conclusion

## Data Sources

We obtained our data from the following source:

- Kaggle Dataset: **(https://www.kaggle.com/datasets/mahdinavaei/marriage-and-divorce-in-iran)**


## Exploratory Data Analysis

Our analysis covers the following aspects:

1. **Time Trends**: How have marriage and divorce rates changed over the past few decades? Are there any noticeable patterns?

2. **Demographic Factors**: We explore how age, education, income, and ethnicity influence marriage and divorce rates.

3. **Geographical Variations**: Are there regional differences in marriage and divorce rates? Which states or regions exhibit unique trends?

4. **Seasonal Patterns**: Do marriage and divorce rates vary by season or month?

## Key Findings

Here are some intriguing findings from our analysis:

- **Marriage Decline**: Marriage rates have declined steadily since the 1980s, with millennials delaying marriage compared to previous generations.

- **Divorce Peaks**: Divorce rates spiked in the 1970s and 1980s but have stabilized since then. Factors like no-fault divorce laws and changing social norms contributed to this trend.

- **Education Matters**: Higher education levels correlate with lower divorce rates. Education seems to act as a protective factor.

## Methodology

Our analysis involved data cleaning, visualization, and statistical tests. We used Python libraries such as pandas, matplotlib, and seaborn. Here's a snippet of code illustrating data preprocessing:

```python
import pandas as pd

# Load marriage and divorce data
marriage_df = pd.read_csv("marriage_data.csv")
divorce_df = pd.read_csv("divorce_data.csv")

# Merge datasets
merged_df = pd.merge(marriage_df, divorce_df, on="year")

# Calculate marriage-to-divorce ratio
merged_df["marriage_divorce_ratio"] = merged_df["marriage_rate"] / merged_df["divorce_rate"]
```
## Conclusion

The upward trend shows that in 1399 (2020), almost half of the couples divorced. As expected, most of the population is from cities; therefore, cities play a greater role than villages. Using lineplots the effect of Marriage rate is higher as it plays a bigger role! Almost 11 times more than divorce rate.

Actually, the divorce rate has been increasing since 1383 (2004). Once again, cities play a greater and more significant role in the divorce rate due to their larger population.
