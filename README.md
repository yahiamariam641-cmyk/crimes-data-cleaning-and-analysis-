# crimes-data-cleaning-and-analysis-
cleaning data for crimes and handling the missing values and duplicats 
# 🚨 Crime Data Cleaning Project

This project focuses on the comprehensive cleaning and initial preprocessing of a crime dataset to ensure data integrity and prepare it for further exploratory data analysis (EDA) or modeling. 🔍

## 📊 Project Overview

The primary objective was to transform a raw crime dataset (`crimes.csv`) into a structured, clean format. The dataset initially contained **185,715 entries** and **12 columns**, covering various aspects of reported crimes such as dates, locations, and victim demographics. 📑

## 🛠️ Technologies Used

* **Python**: Core programming language. 🐍
* **Pandas**: For data manipulation and cleaning. 🐼
* **NumPy**: For numerical operations. 🔢
* **Matplotlib & Seaborn**: For data visualization and inspection. 📈

## 🧹 Data Cleaning Steps

The project followed a systematic approach to data cleaning:

1.  **Initial Data Overview**: Examined the DataFrame's structure, data types, and missing values using `.info()`, `.describe()`, and `.isnull().sum()`. 🕵️‍♀️
2.  **Handling Missing Values**:
    * **Vict Sex & Vict Descent**: Imputed missing entries using the mode of each respective column.
    * **Weapon Desc**: Replaced missing values with the string "Unknown Weapon". 🛠️
3.  **Duplicate Removal**: Performed checks to ensure no duplicate rows existed, maintaining data integrity. 🚫👯
4.  **Standardizing Column Names**: Implemented a cleaning function to convert all column names to lowercase, replace spaces with underscores, and remove special characters. 🔡
5.  **Data Type Conversion**: Converted date-related columns (`daterptd`, `dateocc`) from object types to `datetime64[ns]`. 📅
6.  **Data Consistency Checks**: Analyzed categorical columns to identify unique entries and potential inconsistencies. 🧪

## 💡 Key Findings & Insights

* **Top Crimes**: The most frequent crime types identified were **Identity Theft**, **Battery (Simple Assault)**, and **Burglary from Vehicle**. 🚔
* **Active Areas**: The **Central** and **Southwest** areas recorded the highest number of reported crimes. 📍
* **Data Quality**: While the dataset is now missing-value free, further standardization of the 'Unknown' categories is recommended for more granular analysis. ✨

## 🚀 How to Run

1.  Ensure you have the required libraries installed:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
2.  Load the `crimes (1).ipynb` notebook in Jupyter or Google Colab. 💻
3.  Place the `crimes.csv` file in the appropriate directory or update the load path in the second cell. 📁
