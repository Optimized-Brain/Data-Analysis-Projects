# Customer Churn Analysis

This notebook analyzes customer data to identify factors contributing to churn.

## Data Source

The dataset used in this notebook is the IBM Telco Customer Churn dataset, which is publicly available on Kaggle. It contains information about a fictional telecommunications company's customers and whether they churned or not. The dataset includes various features such as demographic information, services subscribed to, contract details, and payment information.

## Notebook Structure

This notebook is organized into the following sections:

*   **Data Loading:** Loading the dataset and performing initial inspections using `df.head()` and `df.info()`.
*   **Data Cleaning:** Handling missing values in the 'TotalCharges' column and converting its data type to float. Also, converting the 'SeniorCitizen' column to 'yes'/'no' for better readability.
*   **Exploratory Data Analysis (EDA):**
    *   Analyzing the overall churn rate using count plots and pie charts.
    *   Investigating churn based on demographic factors like gender and senior citizenship.
    *   Exploring the relationship between churn and tenure using a histogram.
    *   Examining the impact of contract type on churn.
    *   Visualizing churn across various services (PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies) using count plots.
    *   Analyzing churn based on payment methods.

## Key Findings

Based on the exploratory data analysis, the following key factors appear to influence customer churn:

*   **Overall Churn Rate:** Approximately 26.54% of customers in the dataset have churned.
*   **Gender:** Gender does not appear to be a significant factor influencing churn.
*   **Senior Citizens:** A comparatively greater percentage of senior citizens have churned compared to non-senior citizens.
*   **Tenure:** Customers with shorter tenures (especially 1-2 months) are more likely to churn, while those with longer tenures tend to stay.
*   **Contract Type:** Customers with month-to-month contracts have a significantly higher churn rate compared to those with one-year or two-year contracts.
*   **Services:**
    *   Customers who do not churn tend to have services like PhoneService, InternetService (particularly DSL), and OnlineSecurity.
    *   Churn rates are noticeably higher for customers who do not use or have unavailable services like OnlineBackup, TechSupport, and StreamingTV.
    *   Customers using electronic checks as their payment method are more likely to churn.

## Visualizations

The following visualizations were used to explore the data and understand the factors influencing customer churn:

*   **Count Plots:** Used to show the distribution of customers across various categorical features (e.g., Gender, Senior Citizen, Contract, Services, Payment Method) and to compare the counts of churned versus non-churned customers within these categories.
*   **Pie Chart:** Used to visualize the overall percentage of customers who churned versus those who did not churn.
*   **Histograms:** Used to show the distribution of numerical features like Tenure and how churn varies across different ranges of these features.
*   **Stacked Bar Chart:** Used to compare the proportion of churned and non-churned customers within categories, specifically for the Senior Citizen feature, showing the percentage distribution.


## 7. Getting Started

To run this notebook and replicate the analysis, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Optimized-Brain/Data-Analysis-Projects.git
   cd Data-Analysis-Projects/Customer Churn Data Analysis
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

5. **Navigate to the notebook file** (`Customer Churn Data Analysis.ipynb`) and open it.

6. **Run the cells sequentially** to execute the code and see the results.
