```markdown
# Sales Transaction Dataset

## Overview

This dataset contains **11,865 sales transaction records** from a retail or wholesale operation. Each record represents an individual sales report with details on the product sold, quantity, sales value, salesperson, and a suspicious activity flag.

---

## 📁 File Information

- **File Name**: `Train.xlsx`
- **Sheet Name**: `Sheet 1`
- **Total Records**: 11,865
- **Fields**: 6

---

## 📊 Columns Description

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `ReportID`          | Unique identifier for each sales report (e.g., `Rep10101`)                 |
| `SalesPersonID`     | Identifier for the salesperson (e.g., `C21116`, `C21918`)                  |
| `ProductID`         | Identifier for the product sold (e.g., `PR6112`, `PR6253`)                 |
| `Quantity`          | Number of units sold in the transaction                                    |
| `TotalSalesValue`   | Total monetary value of the sale (in currency units)                       |
| `Suspicious`        | Flag indicating whether the transaction is suspicious (`Yes`, `No`, or `indeterminate`) |

---

## 🧮 Summary Statistics

- **Number of Unique Salespersons**: 16
- **Number of Unique Products**: 200+
- **Suspicious Flag Distribution**:
  - `indeterminate`: 11,787
  - `No`: 72
  - `Yes`: 6

---

## 🧪 Potential Use Cases

This dataset can be used for:

- Fraud detection and anomaly analysis
- Sales performance analysis by salesperson or product
- Inventory and sales trend analysis
- Machine learning models for classifying suspicious transactions

---

## 🔍 Sample Records

| ReportID | SalesPersonID | ProductID | Quantity | TotalSalesValue | Suspicious     |
|----------|---------------|-----------|----------|-----------------|----------------|
| Rep10101 | C21116        | PR6112    | 182      | 1665            | indeterminate  |
| Rep10104 | C21116        | PR6253    | 283      | 4495            | No             |
| Rep11736 | C21976        | PR6590    | 100      | 2515            | Yes            |

---

## 📌 Notes

- The `Suspicious` column is mostly labeled as `indeterminate`, suggesting it may be a target variable for predictive modeling.
- Some transactions involve very high quantities (e.g., 61,216 units) and high sales values (e.g., 415,600), which may be from wholesale or bulk orders.
- The dataset includes a mix of low and high-value transactions, making it suitable for segmentation and outlier detection.

---

## 📈 Suggested Analysis

- Identify top-performing salespeople and products
- Detect outliers in `Quantity` and `TotalSalesValue`
- Build a classifier to predict `Suspicious` transactions
- Explore relationships between product categories and sales trends

---

Let me know if you’d like a deeper analysis or visualizations for this dataset!
```# python-work
