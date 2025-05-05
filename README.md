# 📊 Data Exploration Challenge – Electricity & Gas Billing History (2005–2019)

## 🎯 Objective

This project was part of a hands-on classroom session where students explored and preprocessed **real-world utility billing data** from the Tunisian electricity and gas company. The main goals were to:

* Understand the structure of a raw dataset
* Handle missing data appropriately
* Conduct basic descriptive analysis
* Transform categorical variables
* Build foundational data wrangling skills using **pandas**

## 🗃️ Dataset Description

The dataset contains historical billing records of the Tunisian electricity and gas company's customers, spanning from **2005 to 2019**. Each record reflects a billing transaction for a specific customer and includes categorical and numerical features such as:

* `client_id`
* `counter_type`
* `counter_statue`
* `reading_date`
* `consumption`
* ...and more.

📎 **\[Dataset Link – [https://drive.google.com/file/d/1DVFNq8Gsf9wFZznGafhykVmVHLvAclGo/view]**

---

## ✅ Tasks & Learning Outcomes

### 🔹 1. Load and Preview the Data

* Loaded the dataset and displayed the first 10 records using `client_0_bills = df.head(10)`
* Identified the data type of `client_0_bills` as a `pandas.DataFrame`

### 🔹 2. Dataset Overview

Students answered:

* How many rows and columns are in the dataset?
* How many categorical features are present?
* How much memory does the dataset consume?

This helped introduce them to `df.info()`, `df.shape`, and memory inspection.

### 🔹 3. Missing Values Handling

* Inspected for missing values using `df.isnull().sum()`
* Discussed and applied strategies for handling them (dropping, imputing with mean/median/mode)
* Emphasized **choosing strategies based on the nature and importance of the feature**

### 🔹 4. Descriptive Statistics

* Performed statistical summaries using `df.describe()`
* Helped students interpret measures like mean, std, min, and percentiles for numeric features

### 🔹 5. Subsetting Client Records

* Selected billing history for a specific client (`train_Client_0`) using two methods:

  ```python
  df[df['client_id'] == 'train_Client_0']
  df.query("client_id == 'train_Client_0'")
  ```

### 🔹 6. Encoding Categorical Variables

* Transformed the `counter_type` feature into numerical format
* Introduced techniques like **Label Encoding** and **One-Hot Encoding**
* Explained when to use each approach

### 🔹 7. Feature Dropping

* Removed the `counter_statue` column using `df.drop()`
* Explained how and when to eliminate irrelevant or redundant features

---

## 📘 What Students Practiced

* DataFrame manipulation with `pandas`
* Identifying and handling missing data
* Encoding categorical variables
* Basic data cleaning and feature engineering
* Gaining insights through descriptive statistics

---

## 👩‍🏫 Instructor's Note

This classroom checkpoint was designed to bridge the gap between theoretical preprocessing concepts and **practical data wrangling**. It laid the foundation for deeper explorations, such as outlier detection, time-series analysis, and model preparation in future lessons.


