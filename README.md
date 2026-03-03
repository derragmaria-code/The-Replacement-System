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
* **Observations:** 100,000 records
* **Time Scale:** 1939 – 2026
* **Variables:** 28 (Macroeconomic, Labor, Poverty, and Shadow Economy indicators)



## 💻 Statistical Model
The analysis utilizes Simple Linear Regression (SLR) to model the expansion of the informal sector:

$$Informal\_Economy\_Growth = 19.39 + 0.0586 \times (Currency\_Black\_Market\_Rate\_Gap)$$



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
**DERRAG Mariya** March 2026# The-Replacement-System
Statistical analysis of black markets and informal economic activity in armed conflict (1939–2026). Features a 100,000-record longitudinal dataset and OLS regression models investigating the "Replacement System" theory of war economics.
