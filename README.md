# Task 1 - Data Cleaning & Preprocessing (Netflix Dataset)

## Objective
The aim of this task is to clean and preprocess a raw dataset to make it analysis-ready. I selected the **Netflix Movies and TV Shows dataset** from Kaggle. The dataset contained missing values, duplicates, inconsistent text formats, and unstructured column names. By applying data cleaning techniques, I prepared a structured version suitable for further analysis.

---

## Tools Used
- Python (Pandas, NumPy)
- Google Colab

---

## Steps Performed
1. **Data Loading**  
   Loaded the dataset (`netflix_titles.csv`) using Pandas.

2. **Data Inspection**  
   Checked dataset shape, column types, missing values, and duplicates using `df.info()`, `df.isnull().sum()`, and `df.duplicated().sum()`.

3. **Handling Missing Values**  
   - Filled missing values in `rating` and `country` columns with `"Unknown"`.  
   - Dropped rows where `date_added` was missing.  

4. **Removing Duplicates**  
   Removed duplicate rows with `df.drop_duplicates()`.  

5. **Standardizing Text Values**  
   - Converted `type` column to lowercase.  
   - Removed extra spaces from `title`.  
   - Standardized country names in title case.  

6. **Converting Dates**  
   Converted the `date_added` column into datetime format using `pd.to_datetime()`.  

7. **Renaming Columns**  
   Renamed all columns into lowercase with snake_case formatting.  

---

## Summary of Changes
- Removed duplicate records.  
- Filled missing values in categorical columns with `"Unknown"`.  
- Dropped rows with missing date values.  
- Standardized text formats for consistency.  
- Converted date column into datetime format.  
- Renamed columns for clarity.  

---

## Deliverables
- `netflix_cleaned.csv` → Final cleaned dataset  
- `netflix_cleaning.ipynb` → Notebook with code and steps  
- `README.md` → Documentation  

This exercise improved my skills in handling missing values, duplicates, inconsistent formatting, and preparing data for analysis. It demonstrates the importance of data preprocessing in real-world analytics projects.
