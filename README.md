# Exploratory Data Analysis & Statistical Insights

## Project Overview

This project performs Exploratory Data Analysis (EDA) and statistical analysis on an e-commerce sales dataset.

The objective is to uncover business patterns by analyzing descriptive statistics, distributions, relationships between variables, and statistically testing business hypotheses.

## Dataset

The analysis uses a cleaned e-commerce sales dataset containing:

- 73,699 records
- 24 variables
- Order information
- Sales amount
- Fulfilment details
- Shipping information
- Product categories
- Order status
- Estimated profit metrics

## Analysis Performed

### 1. Descriptive Statistics

Calculated:

- Mean
- Median
- Standard deviation
- Minimum and maximum
- First quartile (25%)
- Third quartile (75%)

### 2. Distribution Analysis

Created:

- Histograms
- Box plots
- Outlier analysis

### 3. Correlation Analysis

A correlation matrix and heatmap were generated to examine relationships between numerical variables.

### 4. Business Hypothesis Testing

Three business hypotheses were statistically tested:

#### Hypothesis 1 — Shipping Service Level vs Sales Amount

A Mann–Whitney U test was used to compare sales-amount distributions between Expedited and Standard orders.

**Result:** Statistically significant difference (p < 0.05).

#### Hypothesis 2 — Fulfilment Type vs Sales Amount

A Mann–Whitney U test was used to compare sales-amount distributions between Amazon and Merchant fulfilment.

**Result:** Statistically significant difference (p = 0.000002).

#### Hypothesis 3 — Fulfilment Type vs Cancellation Rate

A Chi-square test of independence was used to examine the relationship between fulfilment type and cancellation status.

**Result:** Statistically significant association (p < 0.05).

Merchant-fulfilled orders had a higher cancellation rate than Amazon-fulfilled orders.

## Key Business Findings

1. Shipping service level is associated with differences in sales-amount distributions.
2. Fulfilment type is associated with differences in sales-amount distributions.
3. Merchant fulfilment has a higher observed cancellation rate.
4. Average order value varies across fulfilment and shipping-service combinations.
5. T-shirts and Shirts dominate the observed product-category volume.

## Important Note

The dataset does not contain actual cost or profit information. Therefore, estimated profit and estimated profit margin are scenario-based metrics calculated using an assumed 20% margin. They should not be interpreted as actual business profit.

Statistical significance indicates an association or distributional difference and does not establish causation.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Google Colab
- Jupyter Notebook

## Deliverable

The complete analysis is available in:

`EDA_Statistical_Insights.ipynb`
