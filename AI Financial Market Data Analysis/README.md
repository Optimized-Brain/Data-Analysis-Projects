# Realistic Synthetic - AI Financial Market Data Analysis

This notebook analyzes realistic synthetic financial market data for OpenAI, Google, and Meta, focusing on the impact of AI-related R&D spending, revenue, and events on stock prices.

## Table of Contents

1.  [Introduction](#introduction)
2.  [Data Loading and Exploration](#data-loading-and-exploration)
3.  [R&D Spending and Revenue Analysis](#rd-spending-and-revenue-analysis)
4.  [Stock Impact Analysis](#stock-impact-analysis)
5.  [Event Impact Analysis](#event-impact-analysis)
6.  [Correlation Analysis](#correlation-analysis)

## 1. Introduction

This notebook provides an exploratory data analysis of a synthetic dataset containing daily financial market information for three major companies involved in AI: OpenAI, Google, and Meta. The analysis focuses on understanding the relationship between AI-related activities (R&D spending, revenue, and specific events) and their impact on stock performance.

## 2. Data Loading and Exploration

The dataset is loaded into a pandas DataFrame. Initial exploration includes viewing the first few rows, checking data types, and examining the unique values in key columns like 'Company' and 'Year'. The 'Date' column is converted to a datetime object for time-series analysis.

## 3. R&D Spending and Revenue Analysis

This section analyzes the R&D spending and AI revenue for each company. Bar plots are generated to visualize the total R&D spending and AI revenue per company. Additionally, the combined R&D spending and revenue across all companies are plotted year-by-year to show trends over time.

## 4. Stock Impact Analysis

The daily stock impact percentage for each company and overall is visualized as time series plots. This helps to understand the volatility and general trend of stock performance.

## 5. Event Impact Analysis

Specific events listed in the dataset are examined to see their immediate impact on stock prices. Examples include analyzing the stock impact around the release of TensorFlow and GPT-4.

## 6. Correlation Analysis

A heatmap is generated to visualize the correlation matrix of the numerical columns in the dataset. This helps identify potential linear relationships between variables such as R&D spending, AI revenue, AI revenue growth, and stock impact.

## Dataset

The dataset used in this notebook is `ai_financial_market_daily_realistic_synthetic.csv`. It contains the following columns:

*   `Date`: Date of the observation.
*   `Company`: Company name (OpenAI, Google, or Meta).
*   `R&D_Spending_USD_Mn`: Daily R&D spending in USD millions.
*   `AI_Revenue_USD_Mn`: Daily AI revenue in USD millions.
*   `AI_Revenue_Growth_%`: Daily AI revenue growth percentage.
*   `Event`: Description of a specific AI-related event (if any).
*   `Stock_Impact_%`: Daily stock price impact percentage.
*   `Year`: Year of the observation (derived from the 'Date' column).



## 7. Getting Started

To run this notebook and replicate the analysis, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Optimized-Brain/Data-Analysis-Projects.git
   cd Data-Analysis-Projects
   ```

2. **Install the required libraries:**
   It is recommended to use a virtual environment.
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure you have Jupyter Notebook or JupyterLab installed.** If not, you can install it using pip:
   ```bash
   pip install notebook  # or pip install jupyterlab
   ```

4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook  # or jupyter lab
   ```
   This will open the Jupyter interface in your web browser.

5. **Navigate to the notebook file** (`AI Financial Market Data Analysis.ipynb`) and open it.

6. **Run the cells sequentially** to execute the code and see the results.


