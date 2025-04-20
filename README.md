# 🧩 Power Query Automation Project

This project demonstrates how to use Power Query to automate data transformation, including conditional logic and string manipulation.

---

## 📂 What's Included

- **Power Query file**: Contains queries with logic and transformations
- **Dataset folder**: Raw data used for processing
- **Final CSV file**: Cleaned and transformed output

  
Automatically loads and cleans raw data

Applies transformation logic with conditional formulas

Outputs a clean CSV file ready for reporting

---

## 🔍 Key Formulas Used

### 1. `if...else` Logic
Used to categorize data based on conditions:
```powerquery
= Table.AddColumn(Source, "Status", each if [Length of Name] > 10 then "Large name" else "Short name")
### 2. Text.Lenght()
= Table.AddColumn(Source, "NameLength", each Text.Length([Name]))
