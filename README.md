# Session 03 – Data Cleaning and Preprocessing Mini Task

## Project Overview

This project focuses on cleaning and preprocessing a messy workplace dataset for machine learning and data analytics purposes. The task involved identifying common data quality issues, applying suitable cleaning techniques, and preparing the dataset for modelling.

The project was completed as part of the Session 03 Practical Activity on Data Cleaning and Preprocessing.

---

# Objectives

The main objectives of this project were:

* Identify missing values
* Detect duplicate records
* Standardise inconsistent categorical labels
* Check impossible numeric ranges
* Review outliers carefully
* Create encoded categorical features
* Create scaled numerical features
* Improve dataset quality for machine learning

---

# Dataset Information

Dataset used:

* `uk_workplace_data_cleaning_messy_dataset.csv`

The dataset contains workplace-related information including:

* department
* region
* engagement score
* prior python score
* support tickets
* course completion details

---

# Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

# Data Cleaning Steps Performed

## 1. Initial Inspection

Performed:

* dataset shape check
* missing value analysis
* duplicate row detection
* data type inspection

---

## 2. Duplicate Removal

Exact duplicate rows were identified and removed to avoid repeated observations affecting analysis and modelling.

---

## 3. Missing Value Handling

### Categorical Columns

Missing values were replaced using the mode.

### Numerical Columns

Missing values were replaced using the median to reduce the impact of outliers.

---

## 4. Category Standardisation

Inconsistent category labels were corrected.

Examples:

* `operations` → `Operations`
* `finance` → `Finance`
* `REMOTE` → `Remote`

This improved consistency across categorical features.

---

## 5. Impossible Value Detection

Invalid numeric values were identified and corrected.

Examples:

* negative course minutes
* engagement scores above 100
* invalid prior python scores

---

## 6. Feature Engineering

### Encoded Feature

A categorical feature was encoded using Label Encoding.

Created column:

* `department_encoded`

### Scaled Feature

A numerical feature was scaled using StandardScaler.

Created column:

* `prior_python_score_scaled`

---

# Before and After Diagnostics

| Metric         | Before Cleaning | After Cleaning |
| -------------- | --------------- | -------------- |
| Rows           | 102             | 100            |
| Columns        | 12              | 14             |
| Missing Values | Present         | Reduced        |
| Duplicate Rows | Present         | Removed        |

---

# Bias, Signal Preservation, and Leakage

## Bias

Rows were not removed unnecessarily to avoid introducing bias into the dataset.

## Signal Preservation

Outliers were reviewed carefully instead of automatically deleting them to preserve useful information.

## Leakage

The target variable was not modified carelessly during preprocessing to avoid data leakage.

---

# Files Included

| File Name                            | Description                |
| ------------------------------------ | -------------------------- |
| `final_notebook_with_markdown.ipynb` | Complete cleaning notebook |
| `cleaned_uk_workplace_dataset.csv`   | Cleaned dataset            |
| `data_quality_report.docx`           | One-page report            |
| `README.md`                          | Project documentation      |

---

# How to Run the Project

## 1. Clone Repository

```bash
git clone https://github.com/yourusername/session03-data-cleaning.git
```

## 2. Open Project Folder

```bash
cd session03-data-cleaning
```

## 3. Install Required Libraries

```bash
pip install pandas numpy scikit-learn jupyter
```

## 4. Run Notebook

Open Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
final_notebook_with_markdown.ipynb
```

---

# Learning Outcomes

This project improved understanding of:

* data preprocessing
* feature engineering
* missing value handling
* duplicate detection
* machine learning preparation
* reproducible workflows

---

# Author

Jumma Mohammad

---

# License

This project is for educational and portfolio purposes.
