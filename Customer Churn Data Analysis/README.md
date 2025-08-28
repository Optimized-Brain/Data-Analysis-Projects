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


## Instructions

To run this notebook, you will need:

1.  **Python:** Ensure you have Python installed (version 3.6 or higher is recommended).
2.  **Jupyter Notebook:** Install Jupyter Notebook or JupyterLab to open and execute the `.ipynb` file.
3.  **Required Libraries:** Install the necessary Python libraries using pip:
    ```bash
    pip install pandas seaborn matplotlib
    ```
4.  **Open and Run:**
    *   Navigate to the directory where you saved the notebook file (`.ipynb`).
    *   Open your terminal or command prompt in that directory.
    *   Launch Jupyter Notebook or JupyterLab by typing:
        ```bash
        jupyter notebook
        # or
        jupyter lab
        ```
    *   In the Jupyter interface, open the notebook file.
    *   Execute the cells sequentially to run the analysis.