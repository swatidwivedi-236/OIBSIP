# Cleaning Data - Cafe Sales Dataset

## 📌 Objective
This project demonstrates professional-level data cleaning skills by taking a 
deliberately messy retail dataset and systematically transforming it into a 
clean, analysis-ready dataset, with every decision documented along the way.

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Jupyter Notebook

## 📂 Dataset
The dataset (`dirty_cafe_sales.csv`) contains 10,000 rows of synthetic cafe 
sales transactions, intentionally made "dirty" with missing values, 
placeholder errors ("ERROR", "UNKNOWN"), and incorrect data types.

Source: [Kaggle - Cafe Sales Dirty Data for Cleaning Training](https://www.kaggle.com/datasets/ahmedmohamed2003/cafe-sales-dirty-data-for-cleaning-training)

## 🔍 Cleaning Steps Performed
1. **Data Quality Report** – Checked shape, data types, null values, and 
duplicate rows
2. **Fixing Placeholder Errors** – Converted "ERROR" and "UNKNOWN" text 
values into proper missing values (NaN)
3. **Data Type Correction** – Converted Quantity, Price Per Unit, and Total 
Spent to numeric types, and Transaction Date to datetime
4. **Missing Data Handling** – Applied different strategies per column:
   - Text columns (Item, Payment Method, Location) filled with "Unknown"
   - Quantity, Price Per Unit, and Total Spent calculated from each other 
   where possible (since Total = Quantity × Price)
   - Remaining unrecoverable rows and rows with missing dates were dropped
5. **Duplicate Check** – Verified no duplicate rows existed
6. **Standardisation Check** – Verified consistent formatting across text 
columns (no case or spelling issues found)
7. **Outlier Detection** – Used the IQR method to detect outliers in 
Quantity, Price Per Unit, and Total Spent
8. **Before vs After Summary** – Compared row counts, null counts, and data 
type accuracy before and after cleaning

## 📊 Key Findings
- Dataset shrank from 10,000 to 9,485 rows (~5% data loss) after removing 
unrecoverable rows
- Every column had zero missing values after cleaning
- No duplicate rows or formatting inconsistencies were found
- 258 outliers were detected in Total Spent, but retained since they 
represented valid larger transactions (higher quantity × price combinations), 
not data errors

## 📁 Files in this Folder
- `Data_Cleaning_Cafe_Sales.ipynb` – Jupyter Notebook with the full cleaning process
- `dirty_cafe_sales.csv` – Original messy dataset
- `cleaned_cafe_sales.csv` – Final cleaned dataset

## 🎓 About
This project was completed as part of the **AICTE Oasis Infobyte Summer 
Internship Program (OIBSIP)** – Data Analytics Track.

**Author:** Swati Dwivedi
