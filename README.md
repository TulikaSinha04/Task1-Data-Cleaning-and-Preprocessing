# Task1-Data-Cleaning-and-Preprocessing
Clean and prepare a raw dataset (with nulls, duplicates, inconsistent formats).
# Sales Data Cleaning Project

## Overview
This repository contains a cleaned version of the `sales_data_sample.csv` dataset. The dataset has been processed to remove duplicates, handle missing values, standardize text, and ensure consistent formatting for analysis purposes.

---

## Dataset
- **File:** `sales_data_sample.xlsx`
- **Description:** Contains sales data with columns such as order number, order date, product line, customer name, sales amount, and country.
- **Source:** Original dataset `sales_data.csv`.

---

## Steps Taken for Data Cleaning

### 1. Inspect Data
- Checked for missing values in critical columns (`STATE`, `ADDRESSLINE`, `POSTALCODE`).
- Verified consistency in text fields like `PRODUCTLINE` and `COUNTRY`.

### 2. Handle Missing Values
- Deleted rows with excessive missing data.

### 3. Remove Duplicates
- Removed duplicate rows to prevent redundancy.(Not found)

### 4. Standardize Text Values
- Standardize Text Values
TERRITORY:
"NA” → “North America”, "APAC"->"Asia-Pacific"
COUNTRY:
Standardized names: “USA” → “United States”, “UK”→ “United Kingdom”"
.

### 5. Format Dates
- Converted all dates in `ORDERDATE` to `dd-mm-yyyy` format.
- Used `DATEVALUE()` for text-based dates.

### 6. Rename Columns
- Made column headers consistent and easy to use:
  - `ORDERNUMBER` → `order_number`
  - `CUSTOMERNAME` → `customer_name`
  - `SALES` → `sales`

### 7. Check Data Types
---

## Result
The resulting `sales_data_sample.xlsx` file is:
- Free from duplicates and missing critical values.
- Standardized in terms of text, dates, and numbers.
- Ready for analysis in Excel, Python, Power BI, or other tools.

---

## Usage
1. Download `sales_data_sample.xlsx` from this repository.
2. Open in Excel or import into your analysis tool.
3. Use for sales reporting, visualization, or analytics projects.

---

## Notes
- For version control efficiency, CSV format is recommended if frequent updates are expected.
- This project demonstrates basic data cleaning techniques in Excel for beginners.
