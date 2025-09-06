# Customer-Churn-Analysis

# Customer Churn Analysis

This project focuses on analyzing customer churn in a telecommunications company. By understanding the factors that contribute to churn, the company can develop strategies to improve customer retention.

## Dataset

The dataset used in this analysis contains information about customers, including their demographics, services subscribed to, contract details, payment information, and churn status.

## Exploratory Data Analysis (EDA)

The notebook performs an exploratory data analysis to understand the characteristics of customers and identify potential drivers of churn. Key steps include:

- Loading and inspecting the data (`df.info()`, `df.head()`).
- Handling missing values (replacing spaces in 'TotalCharges' with 0 and converting the column to float).
- Checking for duplicate entries.
- Converting the 'SeniorCitizen' column to 'yes'/'no' for better readability.
- Descriptive statistics of numerical features (`df.describe()`).

## Key Findings from Analysis

The analysis revealed several factors associated with customer churn:

- **Overall Churn Rate:** A significant percentage of customers churn (approximately 26.5%).
- **Gender:** Gender does not appear to be a strong predictor of churn.
- **Senior Citizens:** Senior citizens have a higher propensity to churn compared to non-senior citizens.
- **Tenure:** Customers with shorter tenures are more likely to churn. Longer-term customers tend to stay.
- **Contract Type:** Month-to-month contracts are associated with a much higher churn rate than one-year or two-year contracts.
- **Internet Service and Add-on Services:**
    - Customers with Fiber optic internet have a higher churn rate.
    - The absence of services like Online Security, Online Backup, Device Protection, and Tech Support is linked to increased churn.
- **Payment Method:** Customers using Electronic Checks have a higher likelihood of churning.

## Visualizations

The notebook includes several visualizations to illustrate these findings:

- Countplot of customers by churn status.
- Pie chart showing the percentage of customers who churned.
- Countplot of churn by gender.
- Countplot of customers by Senior Citizen status.
- Stacked bar chart showing churn percentage by Senior Citizen status.
- Histogram of tenure distribution by churn status.
- Countplot of churn by contract type.
- Countplots of various service types (PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies) versus churn.
- Countplot of churn by payment method.

## How to Use

1.  Clone the repository.
2.  Ensure you have the necessary libraries installed (pandas, numpy, matplotlib, seaborn).
3.  Place the `churn.csv` file in the same directory as the notebook.
4.  Run the Jupyter Notebook or Google Colab notebook to reproduce the analysis.

## Conclusion

The findings from this analysis provide valuable insights into the characteristics of customers who are likely to churn. This information can be used to develop targeted retention strategies, such as offering incentives for longer contracts, promoting add-on services, and improving the experience for customers using electronic checks.

