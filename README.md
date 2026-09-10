# Telco Customer Churn Analysis

This project explores customer churn in a telecommunications company. The analysis will use customer demographics, subscribed services, contract details, payment methods, tenure, and billing information to understand why customers leave and identify groups that may be at higher risk of churn.

## Dataset

The project uses [`Telco-Customer-Churn.csv`](Telco-Customer-Churn.csv), a customer-level dataset with **7,043 records** and **21 columns**.

The target variable is `Churn`:

- `Yes`: 1,869 customers churned
- `No`: 5,174 customers remained

The dataset includes 11 blank values in `TotalCharges`, which should be treated during data preparation rather than silently converted to zero.

### Main fields

| Category | Fields | Purpose |
| --- | --- | --- |
| Customer profile | `customerID`, `gender`, `SeniorCitizen`, `Partner`, `Dependents` | Describe the customer and household context |
| Account history | `tenure`, `Contract`, `PaperlessBilling`, `PaymentMethod` | Capture customer loyalty and account arrangements |
| Services | `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies` | Describe the products and support services used |
| Charges | `MonthlyCharges`, `TotalCharges` | Measure recurring and accumulated revenue |
| Outcome | `Churn` | Indicates whether the customer left the company |

## Data Source

The dataset is sourced from IBM's telco customer churn example repository:

[IBM Telco Customer Churn dataset](https://github.com/IBM/telco-customer-churn-on-icp4d/blob/master/data/Telco-Customer-Churn.csv)