# War & the Shadow Economy: A Statistical Analysis

This repository contains the dataset, R code, and statistical findings for the research paper: **"War & the Shadow Economy: A Statistical Analysis of Black Markets and Informal Economic Activity in Armed Conflict."**

## 📌 Research Overview

Traditional economics views war as a period of destruction. This research reframes war as an **economic transformation**, demonstrating that economic activity is not destroyed but redirected into a shadow system that operates independently of formal conditions.

### Key Findings

* **The Structural Constant:** War profiteering occurs in **70%** of conflicts, with <2% variance across all global regions.
* **The War Intercept:** Regression analysis reveals a baseline informal economy growth of **19.39pp** driven solely by the state of conflict.
* **Economic Decoupling:** Standard indicators (GDP, Inflation) show near-zero correlation ($r \approx 0$) with informal growth. The **Currency Black Market Gap** ($r = 0.60$) is the sole measurable predictor.

## 📊 Dataset Specifications

* **Name:** War Economic & Livelihood Impact Dataset
* **Source:** [Kaggle — War Economic and Livelihood Impact Dataset](https://www.kaggle.com/datasets/likithagedipudi/war-economic-and-livelihood-impact-dataset)
* **Observations:** 100,000 records
* **Time Scale:** 1939 – 2026
* **Variables:** 28 (Macroeconomic, Labor, Poverty, and Shadow Economy indicators)

## 💻 Statistical Model

The analysis utilizes Simple Linear Regression (SLR) to model the expansion of the informal sector:

$$Informal\_Economy\_Growth = 19.39 + 0.0586 \times (Currency\_Black\_Market\_Rate\_Gap)$$

| Metric | Value |
|---|---|
| R² | 0.3635 |
| F-statistic | 57,100 (p < 2.2×10⁻¹⁶) |
| Durbin-Watson | 2.0008 |

## ⚠️ Limitations

This research has several limitations that should be considered when interpreting the findings:

1. **Moderate explanatory power.** The model's R² of 0.364 means approximately 64% of the variance in informal economy growth remains unexplained. Factors such as conflict duration, institutional collapse, geographic isolation, and governance quality are not captured by the single-predictor model.

2. **Simple Linear Regression and omitted variable bias.** Using a single predictor (currency black market gap) on 100,000 observations risks omitted variable bias. A multivariate regression including additional controls (e.g., conflict type, duration, pre-war institutional strength) would produce more reliable estimates.

3. **Correlation vs. causation.** The regression establishes a statistically significant association between the currency black market gap and informal economy growth, but does not establish causation. The directional relationship could be bidirectional — shadow economy expansion may itself widen the currency gap.

4. **Profiteering measurement.** The claim that profiteering occurs in 70% of conflicts is presented without a detailed explanation of how this variable was operationalized in the dataset. The measurement definition should be made explicit.

5. **No multivariate comparison.** The paper claims the currency gap is the "primary measurable predictor" of shadow economy growth, but does not test this claim against other predictors in a multivariate model. This comparison would be necessary to substantiate the primacy claim.

6. **Dataset provenance.** The dataset spans 1939–2026 across diverse conflict types and regions. Differences in how informal economic activity was measured or estimated across historical periods and geographies may introduce systematic bias.

## 🛠️ Requirements

Analysis was performed in **R 4.x** using the following packages:

* `dplyr` / `tidyr` - Data manipulation
* `ggplot2` - Visualizations
* `lmtest` - Diagnostic tests (Durbin-Watson, etc.)

## 📂 Repository Structure

* `/data`: Contains `war_economic_impact_dataset.csv`.
* `/scripts`: R scripts for data cleaning and regression analysis.
* `/results`: Full statistical outputs and high-resolution plots.

## Author

**DERRAG Mariya** — March 2026 activity in armed conflict (1939–2026). Features a 100,000-record longitudinal dataset and OLS regression models investigating the "Replacement System" theory of war economics.
