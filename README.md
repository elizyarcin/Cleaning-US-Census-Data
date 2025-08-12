# Cleaning US Census Data 🗂️

A comprehensive data cleaning and preprocessing project for the **US Census dataset**, preparing it for insightful analysis and visualization.

---

## 🚀 Project Overview

The US Census dataset provides demographic information per state, including population, ethnicity distribution, income, and gender data.  
Raw data contains formatting inconsistencies such as `%`, `$`, commas, and combined gender info.

This project addresses:

- 🗑️ Removing redundant columns  
- 🔄 Converting strings with special characters (`%`, `$`) into numeric types  
- ✂️ Splitting combined columns (`GenderPop`) into separate `Male` and `Female` columns  
- 🛠️ Handling missing or malformed data  
- 🧹 Removing duplicates  
- 📊 Preparing clean data ready for visualization and analysis  

---

## 📋 Dataset Summary

| Column    | Description                        |
| --------- | -------------------------------- |
| State     | Name of the US state              |
| TotalPop  | Total population                  |
| Hispanic  | % of Hispanic population          |
| White     | % of White population             |
| Black     | % of Black population             |
| Native    | % of Native American population   |
| Asian     | % of Asian population             |
| Pacific   | % of Pacific Islander population |
| Income    | Median income (in US dollars)     |
| GenderPop | Combined male and female counts   |

---

## 🧹 Data Cleaning Pipeline

1. **Drop unnecessary columns** like `Unnamed: 0`.  
2. **Clean percentage columns:** remove `%`, convert to floats.  
3. **Clean income column:** strip `$` and `,`, convert to floats.  
4. **Split `GenderPop`:** create `Male` and `Female` integer columns.  
5. **Handle missing data:** fill or remove null values as appropriate.  
6. **Remove duplicate entries** to ensure data integrity.  
7. **Convert all columns** to appropriate data types for analysis.  

---

## 💻 How to Use

Run the cleaning notebook:

```bash
jupyter notebook Cleaning-US-Census-Data.ipynb

