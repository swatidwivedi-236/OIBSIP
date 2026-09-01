# EDA on Retail Sales Data

## 📌 Objective
This project performs a thorough Exploratory Data Analysis (EDA) on a retail 
sales dataset to uncover patterns, customer behaviour trends, and actionable 
business insights.

## 🛠️ Tech Stack
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📂 Dataset
The dataset (`retail_sales_dataset.csv`) contains 1000 transaction records with 
9 columns: Transaction ID, Date, Customer ID, Gender, Age, Product Category, 
Quantity, Price per Unit, and Total Amount.

Source: [Kaggle - Retail Sales Dataset](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset/data)

## 🔍 Analysis Performed
1. **Initial Inspection** – Checked dataset shape, column data types, and null values
2. **Descriptive Statistics** – Mean, median, mode, and standard deviation for all numerical columns
3. **Time Series Analysis** – Monthly and quarterly sales trends using line charts
4. **Customer Demographics** – Age distribution and gender breakdown
5. **Product Analysis** – Sales count and revenue by product category
6. **Correlation Heatmap** – Relationship between numerical variables
7. **Extra Insight** – Average spending by age group

## 📊 Key Findings
- Sales fluctuate significantly through the year, peaking in May and dipping in September
- Customer base is evenly split by gender and spread across all age groups
- Electronics generates the highest revenue despite having fewer sales than Clothing
- Price per Unit and Total Amount are strongly correlated (0.85)
- Customers aged 18-25 spend the most on average per transaction

## 💡 Business Recommendations
1. Focus marketing efforts on the 18-35 age group, as they spend the most per transaction
2. Promote Electronics more aggressively since it drives the highest revenue
3. Run promotions during September to counter the seasonal sales dip

## 📁 Files in this Folder
- `EDA_Retail_Sales.ipynb` – Jupyter Notebook with the full analysis
- `retail_sales_dataset.csv` – Dataset used for the analysis

## 🎓 About
This project was completed as part of the **AICTE Oasis Infobyte Summer 
Internship Program (OIBSIP)** – Data Analytics Track.

**Author:** Swati Dwivedi
