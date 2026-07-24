# 🧹 Project 1 – Data Cleaning & Preparation

## 📌 Internship Details

- **Organization:** DecodeLabs
- **Program:** Industrial Training Kit 2026
- **Domain:** Data Analytics
- **Project:** Project 1 – Data Cleaning & Preparation
- **Intern:** Ishika Prajapati

---

# 📖 Project Overview

This project focuses on cleaning and preparing a raw dataset for further analysis. The objective is to improve data quality by identifying and correcting common data issues such as missing values, duplicate records, inconsistent formatting, and invalid entries.

The cleaned dataset is suitable for future analytical tasks such as visualization, reporting, and predictive modeling.

---

# 🎯 Objective

The primary goals of this project are to:

- Handle missing values
- Remove duplicate records
- Validate unique identifiers
- Standardize date formats
- Clean text fields
- Verify numeric consistency
- Produce a clean, analysis-ready dataset

---

# 📂 Project Structure

```
Project1_Data_Cleaning/
│
├── Dataset for Data Analytics.xlsx
├── Dataset for Data Analytics_CLEANED_using_python_script.xlsx
├── Project1_Data_Cleaning.py
├── Project1_Data_Cleaning.ipynb
└── README.md
```

---

# 🛠 Technologies Used

- Python 3
- Pandas
- OpenPyXL
- Jupyter Notebook
- Visual Studio Code

---

# 📊 Dataset Information

The dataset contains customer order information with **1,200 records** and **14 columns**.

### Features

- OrderID
- Date
- CustomerID
- Product
- Quantity
- UnitPrice
- ShippingAddress
- PaymentMethod
- OrderStatus
- TrackingNumber
- ItemsInCart
- CouponCode
- ReferralSource
- TotalPrice

---

# 🔍 Data Cleaning Process

## 1. Initial Data Audit

Performed an initial inspection to identify:

- Missing values
- Duplicate rows
- Duplicate Order IDs
- Invalid ID formats
- Incorrect TotalPrice calculations
- Data types

---

## 2. Duplicate Removal

Removed:

- Fully duplicated rows
- Duplicate Order IDs while keeping the first occurrence

---

## 3. Missing Value Handling

Missing values in the **CouponCode** column were replaced with:

```
No Coupon
```

This preserves all records while eliminating null values.

---

## 4. Date Standardization

Converted all date values into a consistent format using Pandas DateTime.

---

## 5. Text Cleaning

Standardized text columns by:

- Removing leading spaces
- Removing trailing spaces
- Standardizing formatting

Applied to:

- Product
- ShippingAddress
- PaymentMethod
- OrderStatus
- CouponCode
- ReferralSource
- OrderID
- CustomerID
- TrackingNumber

---

## 6. Numeric Validation

Verified:

- UnitPrice precision
- TotalPrice precision
- TotalPrice = Quantity × UnitPrice

Rounded monetary values to two decimal places.

---

## 7. ID Validation

Validated the format of:

### OrderID

```
ORD######
```

### CustomerID

```
C#####
```

### TrackingNumber

```
TRK########
```

---

## 8. Verification

Final validation ensured:

- No duplicate Order IDs
- No malformed IDs
- No remaining null values
- Correct TotalPrice calculations
- Clean dataset ready for analysis

---

# ✅ Output

The project generates:

### Clean Dataset

```
Dataset for Data Analytics_CLEANED_using_python_script.xlsx
```

Contains:

- Cleaned dataset
- Cleaning log

---

# 📈 Skills Demonstrated

- Data Cleaning
- Data Validation
- Missing Value Treatment
- Duplicate Detection
- Data Quality Assessment
- Pandas
- Excel Processing
- Data Preparation
- Python Programming

---

# ▶️ How to Run

1. Install the required libraries.

```bash
pip install pandas openpyxl
```

2. Place the dataset in the project folder.

3. Run the script.

```bash
python Project1_Data_Cleaning.py
```

4. The cleaned Excel file will be generated automatically.

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Inspecting raw datasets
- Identifying common data quality issues
- Cleaning and transforming data using Python
- Preparing datasets for downstream analytics
- Creating reusable and structured data-cleaning workflows

---

# 👩‍💻 Author

**Ishika Prajapati**

Data Analytics Intern  
DecodeLabs Industrial Training Program 2026

---

# ⭐ Acknowledgement

This project was completed as part of the **DecodeLabs Industrial Training Kit 2026** under the **Data Analytics** domain. It demonstrates the practical application of data cleaning techniques using Python and Pandas.