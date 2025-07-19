# Airbnb NYC 2019 – Data Cleaning Project
# Internship Task – Oasis Infobyte (Data Analyst)
This project involves cleaning and preprocessing the 2019 Airbnb listing dataset for New York City. The goal is to ensure the dataset is accurate, consistent, and ready for data analysis or machine learning tasks.

# Dataset Description
- **Source:** [Airbnb NYC 2019 Dataset](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)
- **Context:** The dataset contains detailed information about Airbnb listings in NYC, including host details, location, price, availability, and review metrics

# Objectives
- Ensure **data integrity**
- Handle **missing values**
- Remove **duplicate records**
- **Standardize** column formatting
- Detect and address **outliers**

# Steps Performed

### 1. Importing Libraries & Dataset
- Loaded dataset using `pandas`
- Inspected structure with `.info()`, `.describe()`, and `.isnull().sum()`

### 2. Handling Missing Values
- Filled `reviews_per_month` with 0
- Dropped rows missing `name` or `host_name`
- Converted `last_review` to datetime or dropped it (optional)

### 3. Duplicate Removal
- Removed duplicate rows using `.drop_duplicates()`

### 4. Column Standardization
- Standardized column names to lowercase with underscores

### 5. Outlier Detection
- Used boxplot to visualize extreme values in `price`
- Removed outliers above $1000 (adjustable)

# Cleaned Dataset

-  Final shape: `after cleaning`
-  0 missing values
- Ready for analysis or visualization

#  Files Included

| File Name                     | Description                      |
|------------------------------|----------------------------------|
| `AB_NYC_2019_cleaned.csv`    | Final cleaned dataset             |
| `Airbnb_Data_Cleaning.ipynb` | Jupyter Notebook with all steps  |
| `README.md`                  | This file                        |

# Tools Used

- Python 
- Pandas
- Matplotlib & Seaborn
- Jupyter Notebook
