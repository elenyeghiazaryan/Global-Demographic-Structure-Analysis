# Global Demographic Structure Analysis (GDS-2025)

## Project Overview
The global population is growing inconsistently, creating significant disparities in density, fertility, and urbanization across 233 countries. This project provides a comprehensive statistical analysis of these factors to uncover patterns essential for infrastructure, healthcare, and economic planning.

Using a multi-stage data pipeline, this project transforms raw web-scraped data into actionable insights through descriptive statistics, hypothesis testing, and advanced visualizations.

## Key Features
* **Automated Data Scraping:** Fetches real-time data from Worldometers using `BeautifulSoup` and `requests`.
* **Robust Data Cleaning:** Handles missing values, removes duplicates, and cleans non-numeric characters (e.g., symbols, percent signs) for reliable analysis.
* **Feature Engineering:** Includes custom metrics like the **Urban-Rural Ratio** to better understand demographic distributions.
* **Statistical Analysis:** * **Descriptive Stats:** Mean, Median, and Standard Deviation to identify skewness in global population.
    * **Normality Testing:** Shapiro-Wilk tests for distribution analysis.
    * **Hypothesis Testing:** T-tests and ANOVA to validate relationships between fertility, urbanization, and median age.
* **Advanced Visualizations:** Utilizing `Seaborn` and `Matplotlib` for heatmaps, scatter plots, and distribution curves.

## Analysis Highlights
* **The Fertility-Age Link:** Correlation analysis reveals a strong negative relationship ($r = -0.85$) between fertility rate and median age.
* **Urbanization Impact:** ANOVA testing confirms that countries with higher urbanization levels significantly differ in median age compared to rural-majority nations.
* **Skewed Distributions:** Global data is heavily right-skewed; a few outliers (like India and China) pull the mean far above the global median.

## Technical Stack
* **Language:** Python
* **Libraries:** * Data Handling: `pandas`, `numpy`
    * Scraping: `BeautifulSoup4`, `requests`
    * Statistical Modeling: `scipy`, `sklearn`
    * Visualization: `matplotlib`, `seaborn`

## Project Structure
1.  **Stage 1: Data Scraping** – Extracting worldwide population data.
2.  **Stage 2: Data Cleaning** – Correcting data types and handling missing values.
3.  **Stage 3: Preprocessing** – Scaling, normalization, and feature engineering.
4.  **Stage 4: EDA** – Correlation matrices and statistical testing.
5.  **Stage 5: Visualization** – Generating histograms, box plots, and heatmaps.

## Authors
* **Elen Yeghiazaryan**
* **Milena Yeganyan**

**Course:** Algorithms and Programming Language (APL)  
**Professor:** Varazdat Avetisyan  
**Date:** November 2025
