# Customer_Churn_prevention_Insights 🤖

## Customer Churn Prediction

In this project, we aim to build a classification model to predict the likelihood of customer churn for a telecom company (Vodafone). Using Supervised Machine Learning, we will explore how churn analytics can help businesses proactively identify customers at risk of leaving, optimize retention efforts, and create strategies to enhance customer loyalty.

### Project Overview

Customer churn is a significant issue for subscription-based industries, and this predictive model provides a data-driven solution to address it. By identifying customers who are likely to churn, businesses can take steps to retain them before it's too late. The project follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework to analyze customer churn within the Vodafone network.

### Table of Contents 🔖
- [Project Overview](#project-overview)
- [Project Links](#project-links)
- [Tools Used](#tools-used)
- [Dataset](#dataset)
- [Process](#process)
- [Model Performance](#model-performance)
- [Dashboard](#dashboard)
- [Conclusion and Recommendations](#conclusion-and-recommendations)

---

## Project Links 🔗
- **[Customer Churn Classification Model](#)**: Jupyter Notebook containing model training and evaluation.
- **[Medium Article](#)**: A detailed article explaining the project, methodology, and results.
- **[Power BI Dashboard](#)**: View the interactive Power BI dashboard showcasing the churn analysis.

---

## Tools Used 🧰
- **VS Code**: Code editor used for development.
- **pandas**: Data manipulation and analysis.
- **numpy**: Numerical computations.
- **python**: Programming language.
- **jupyter**: Interactive environment for running Python code.

---

## Dataset 💾

The dataset contains various features that help predict customer churn. Below is a description of the dataset's columns:

| **Feature Name**        | **Description**                                                              | **Data Type**   |
|-------------------------|------------------------------------------------------------------------------|-----------------|
| customerID              | Unique customer identifier                                                   | Categorical     |
| gender                  | Whether the customer is female or male                                        | Categorical     |
| SeniorCitizen           | Whether the customer is a senior citizen (1, 0)                              | Numeric, int    |
| Partner                 | Whether the customer has a partner                                           | Categorical     |
| Dependents              | Whether the customer has dependents                                          | Categorical     |
| tenure                  | Number of months the customer has stayed with the company                    | Numeric, int    |
| PhoneService            | Whether the customer has phone service                                       | Categorical     |
| MultipleLines           | Whether the customer has multiple lines                                      | Categorical     |
| InternetService         | Customer’s internet service provider (DSL, Fiber optic, No)                  | Categorical     |
| OnlineSecurity          | Whether the customer has online security                                     | Categorical     |
| OnlineBackup            | Whether the customer has online backup                                       | Categorical     |
| DeviceProtection        | Whether the customer has device protection                                   | Categorical     |
| TechSupport             | Whether the customer has tech support                                        | Categorical     |
| streamingTV             | Whether the customer has streaming TV                                        | Categorical     |
| streamingMovies         | Whether the customer has streaming movies                                    | Categorical     |
| Contract                | The contract term of the customer (Month-to-month, One year, Two year)      | Categorical     |
| PaperlessBilling        | Whether the customer has paperless billing                                   | Categorical     |
| PaymentMethod           | Customer’s payment method (Electronic check, Mailed check, Bank transfer, Credit card) | Categorical |
| MonthlyCharges          | The amount charged to the customer monthly                                   | Numeric, int    |
| TotalCharges            | Total amount charged to the customer                                          | Object          |
| Churn                   | Whether the customer churned or not (Yes or No)                              | Categorical     |

---

## Process

1. **Data Collection**: Data is pulled from multiple sources, including a remote SQL server database.
2. **Hypothesis Development**: Formulating analytical questions to explore and test with the data.
3. **Data Preprocessing & Cleaning**: Handling missing values, encoding categorical variables, and ensuring the data is ready for modeling.
4. **Exploratory Data Analysis (EDA)**: Performing univariate, bivariate, and multivariate analysis to uncover patterns and relationships.
5. **Data Visualization**: Creating visualizations to answer the analytical questions using Power BI.
6. **SMOTE Algorithm for Oversampling**: Balancing the dataset to handle class imbalances.
7. **Feature Engineering & Scaling**: Creating new features and scaling the data for better model performance.
8. **Model Training & Evaluation**: Training various machine learning models and evaluating them using appropriate metrics.
9. **Hyperparameter Tuning**: Fine-tuning the model to achieve better performance.
10. **Prediction & Model Improvements**: Testing the model and making improvements based on its performance.
11. **Conclusion**: Summarizing findings and writing an article on the results.

---

## Model Performance 📊

- **Accuracy Scores**: The trained models achieved an accuracy of around **86%** on the test data after hyperparameter tuning. Random Forest and other ensemble methods performed well, with ensemble methods showing superior results compared to single classifiers.
- **Key Features**: 
  - The number of months a customer has stayed with the company (tenure) and the contract type (contract) were found to be the most significant predictors of churn.
  - **Accuracy Score after Hyperparameter Tuning**: ~86%

---

## Dashboard 📺

An interactive **Power BI** dashboard is created to visualize the customer churn analysis. This dashboard allows users to explore the data and observe trends related to customer churn, helping businesses make data-driven decisions.

[View the interactive dashboard here](Churn_Dashboard.pdf).

---

## Conclusion and Recommendations

Based on the analysis, we recommend the following:

1. **Enhance Early Customer Experience**:
   - Customers in their first 5-10 months show a higher churn rate, suggesting that improving onboarding processes and addressing customer concerns during this period will boost customer retention.

2. **Promote Long-Term Contracts**:
   - Customers with month-to-month contracts have a higher churn rate. Encouraging customers to opt for one-year or two-year contracts could potentially reduce churn and foster customer loyalty.

3. **Model Insights**:
   - Ensemble methods, such as Random Forest, performed well in classification tasks, and hyperparameter tuning helped achieve a slight performance improvement.
   - Hyperparameter tuning doesn’t always drastically improve model performance, but it does offer slight improvements when done correctly.


