# Employee Data Preprocessing Pipeline

This repository showcases a complete data preprocessing pipeline applied to a sample employee dataset. The goal is to prepare the dataset for machine learning models by addressing common data quality issues such as missing values, outliers, inconsistent data formats, and categorical variables.

---

## Dataset Description

The dataset includes fictional employee information with the following columns:

| Column      | Description                  |
|-------------|------------------------------|
| Name        | Employee's full name         |
| Age         | Employee's age in years      |
| Gender      | Gender of the employee       |
| Salary      | Annual salary in USD         |
| Department  | Department within the company|

---

##  Preprocessing Workflow

### 1. Handling Missing Values
- Visualized null entries using:
  - `missingno`
  - `seaborn`
- Imputation techniques:
  - Age: Filled with **median**
  - Gender: Filled with **mode**
  - Salary: Filled with **mean**

---

###  2. Outlier Detection
- Visualized with:
  - Boxplot
  - Scatterplot
- Outlier detection techniques used:
  - **IQR (Interquartile Range)**
  - **Z-score**
  - **Isolation Forest**

---

###  3. Categorical Encoding
- `Gender` encoded using **LabelEncoder**
- `Department` encoded using:
  - **Pandas `get_dummies`**
  - **OneHotEncoder** (scikit-learn)

---

### 4. Feature Scaling
- **StandardScaler** used for standardization:
  - `Age_std`, `Salary_std`
- **MinMaxScaler** used for normalization:
  - `Age_norm`, `Salary_norm`

---

##  Libraries Used

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `missingno`
- `scikit-learn`
- `scipy`
