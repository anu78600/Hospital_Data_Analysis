# Hospital Data Cleaning & Preparation — Excel

##  Project Overview

The original dataset contained inconsistent formatting, missing values, unnecessary characters, inconsistent capitalization, and mixed date formats.

I cleaned and standardized the dataset using **Microsoft Excel**, making it easier to use for further analysis and visualization.

### Dataset

* **Rows:** 55,505
* **Columns:** 15
* **Original Format:** CSV
* **Cleaning Tool:** Microsoft Excel
* **Final Format:** Excel (.xlsx)

---

## 🧹 Data Cleaning Process

### 1. Identifying Missing Values

Used Excel filters and **Go To Special** to identify blank cells across the dataset.

Handled missing values by replacing appropriate blanks with:

> `Unknown`

This ensured the final dataset did not contain empty cells.

---

### 2. Find & Replace

Used **Find & Replace** to remove unwanted characters and standardize inconsistent values.

Examples included:

* Removing unnecessary symbols
* Removing extra characters from names
* Cleaning hospital names
* Cleaning doctor names
* Standardizing inconsistent text values

---

### 3. Handling Text Formatting

Used Excel formulas and formatting techniques to improve consistency.

#### `TRIM()`

Used to remove unnecessary spaces from text.

```excel
=TRIM(A2)
```

#### `PROPER()`

Used to standardize capitalization.

```excel
=PROPER(A2)
```

These formulas helped convert inconsistent text such as:

```text
dAnnY SMiTH
```

into:

```text
Danny Smith
```

---

### 4. Standardizing Gender Values

Converted inconsistent gender representations into standardized values.

Examples:

```text
M → Male
FEMALE → Female
```

Final values were standardized as:

* Male
* Female

---

### 5. Cleaning Dates

The dataset contained dates in different formats.

Examples included:

```text
2024.01.31
09/22/2022
02-02-2024
```

These were converted into a consistent date format:

```text
YYYY-MM-DD
```

---

### 6. Cleaning Billing Amounts

The original billing values contained currency text such as:

```text
18856.281305978155 USD
```

The unnecessary currency text was removed so the column could be treated as a numerical field.

Example:

```text
18856.281305978155 USD
        ↓
18856.281305978155
```

---

### 7. Cleaning Names & Organizations

Removed unnecessary characters and formatting issues from:

* Patient names
* Doctor names
* Hospital names

For example:

```text
Matthew Smith ##  Sons and Miller,,
```

was cleaned into standardized values such as:

```text
Matthew Smith
Sons and Miller
```

---

### 8. Standardizing Test Results

Inconsistent test-result values were standardized.

For example:

```text
N
```

was converted to:

```text
Normal
```

and missing/unknown values were represented consistently as:

```text
Unknown
```

---

##  Excel Techniques Used

During this project, I practiced:

* Find & Replace
* Go To Special
* Filters
* Sorting
* Handling blank values
* `TRIM()`
* `PROPER()`
* Text cleaning
* Date formatting
* Number formatting
* Data standardization
* Removing unnecessary characters
* Identifying inconsistent values
* Preparing data for analysis

---

##  Dataset Columns

| Column             | Description             |
| ------------------ | ----------------------- |
| Name               | Patient name            |
| Age                | Patient age             |
| Gender             | Patient gender          |
| Blood Type         | Patient blood group     |
| Medical Condition  | Medical condition       |
| Date of Admission  | Admission date          |
| Doctor             | Assigned doctor         |
| Hospital           | Hospital name           |
| Insurance Provider | Insurance provider      |
| Billing Amount     | Hospital billing amount |
| Room Number        | Assigned room           |
| Admission Type     | Type of admission       |
| Discharge Date     | Patient discharge date  |
| Medication         | Medication provided     |
| Test Results       | Test result             |

---

##  Before vs After

### Before Cleaning

The original dataset contained:

* Missing values
* Inconsistent capitalization
* Extra spaces
* Unwanted characters
* Mixed date formats
* Currency text inside numerical values
* Inconsistent categorical values

### After Cleaning

The final dataset contains:

* Consistent formatting
* Standardized text
* Standardized dates
* Clean numerical values
* Consistent categorical values
* No blank cells
* Analysis-ready data

---

## 📁 Project Files

```text
Hospital-Data-Cleaning/
│
├── hospital_data_unclean.csv
├── hospital_data_cleaned.xlsx
└── README.md
```

---

##  Key Learning

This project helped me understand that **data analysis starts before the dashboard or SQL query**.

Clean and consistent data is essential for reliable analysis.

Through this project, I learned how to approach messy real-world data in Excel and prepare it for the next stage of analysis.

> **Clean data → Better analysis → Better decisions**

---

##  Next Step

The cleaned dataset can now be used for:

* Exploratory Data Analysis
* Excel analysis
* Power BI dashboards
* SQL analysis
* Data visualization
* Business insights

---

## 👨‍💻 Skills Demonstrated

**Microsoft Excel | Data Cleaning | Data Preparation | Data Standardization | Data Quality | Missing Value Handling | Text Functions | Filtering | Find & Replace | Data Analysis**

---

### ⭐ Project Status

**Completed — Data Cleaning & Preparation**
