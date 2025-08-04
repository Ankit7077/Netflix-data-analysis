# 📊 Netflix Data Analysis Project

This project involves exploratory data analysis (EDA) on the **Netflix titles dataset**, which contains information about movies and TV shows available on the platform. The goal is to clean the data, handle missing values, standardize columns, and extract meaningful insights.

---

## 📁 Dataset

- **Source**: Netflix Titles (CSV)
- **Fields Included**:
  - Title, Type (Movie/TV Show), Director, Cast
  - Country, Date Added, Release Year
  - Rating, Duration, Genre (`listed_in`)
  - Description

---

## 🧹 Data Cleaning Performed

### ✅ 1. Missing Values
- Identified using `.isnull()`
- Columns like `director`, `cast`, `country`, and `date_added` had null entries
- Treated missing values using default methods or left as `NaT/NaN` for further handling

### ✅ 2. Duplicate Removal
- Removed duplicate rows using `.drop_duplicates()`

### ✅ 3. Text Standardization
- Converted all text fields to **lowercase**
- Stripped extra whitespace
- Standardized entries like `country`, `rating`, and `listed_in`

### ✅ 4. Date Conversion
- Converted the `date_added` column to proper **datetime** format using:
  ```python
✅ 5. Column Normalization
Renamed all columns to snake_case (e.g., Date Added → date_added)

Replaced spaces and capital letters for easier code access

✅ 6. Data Type Fixes
Converted numerical-looking strings to integers where appropriate (e.g., release year)

Ensured correct types for analysis (int, datetime, str, etc.)
