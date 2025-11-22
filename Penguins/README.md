

# 🧹 Data Cleaning with Pandas: Handling Missing Values

This repository contains a Jupyter Notebook (`03_Pandas_DataFrames_Continued_01_JennyGUO.ipynb`) demonstrating key techniques in the **Pandas** library for identifying, counting, and handling missing data values in a DataFrame.

***

## 📊 Data Source: `penguins.csv`

The data used in this project is sourced from the `penguins.csv` file. It is a well-known dataset containing biological and geographic measurements for three species of penguins.

### 🐧 Table Structure and Schema

The dataset includes the following columns. Missing values are represented by **NA** in the raw CSV.

| Column Name | Description | Data Type | Notes |
| :--- | :--- | :--- | :--- |
| `species` | The species of the penguin. | Object (String) | |
| `island` | The island where the penguin was found (Torgersen, Biscoe, or Dream). | Object (String) | |
| `bill_length_mm` | Length of the bill (culmen) in millimeters. | Numeric (Float) | ⚠️ Contains missing values. |
| `bill_depth_mm` | Depth of the bill (culmen) in millimeters. | Numeric (Float) | ⚠️ Contains missing values. |
| `flipper_length_mm` | Length of the flipper in millimeters. | Numeric (Integer) | ⚠️ Contains missing values. |
| `body_mass_g` | Body mass in grams. | Numeric (Float) | ⚠️ Contains missing values. |
| `sex` | The sex of the penguin (male or female). | Object (String) | ⚠️ Contains missing values. |
| `year` | The year of the observation. | Numeric (Integer) | |

***

## 🐍 Key Python Functions Used

The notebook primarily uses the `pandas` library (imported as `pd`) to manipulate and analyze data.

### 💾 1. Data Loading and Inspection

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`import pandas as pd`** | 🐼 | Imports the pandas library for data manipulation. |
| **`pd.read_csv('filename.csv')`** | 📄 | Loads data from a CSV file into a Pandas DataFrame. |
| **`.info()`** | ℹ️ | Provides a summary of the DataFrame, including data types and a count of **non-null** values. |
| **`.mean()`** | 🔢 | Calculates the average of a numeric column, ignoring `NaN` values. |
| **`.value_counts(dropna=False)`** | 📈 | Counts unique values in a Series, and explicitly includes the count of missing values (`None`/`NaN`). |

### 🕵️‍♀️ 2. Identifying Missing Values

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`.isna()`** | 🤔 | Returns a boolean DataFrame/Series where `True` indicates a missing value. |
| **`.isna().sum()`** | ➕ | Counts the total number of missing values per **column** (default `axis=0`). |
| **`.isna().sum(axis=1)`** | 📏 | Counts the number of missing values per **row**. |
| **`.isna().mean()`** | 💯 | Calculates the **proportion** (percentage) of missing values per column. |

### 🗑️ 3. Cleaning and Handling Missing Data

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`.dropna()`** | ✂️ | Removes rows that contain at least one missing value. |
| **`.dropna(axis=1)`** | 🔪 | Removes columns that contain at least one missing value. |
| **`.dropna(subset=[...])`** | 🎯 | Removes rows that have missing values **only** in the specified subset of columns. |
| **`.fillna(value)`** | 🔄 | Replaces missing values (`NaN`/`None`) in the DataFrame with a specific static `value`. |
| **`.drop(columns=[...])`** | ❌ | Removes one or more specified columns from the DataFrame. |

### ✨ 4. Data Manipulation Utilities

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`.set_index('column_name')`** | 🏷️ | Sets a column as the index for the DataFrame. |
| **`.sort_values(ascending=False)`** | ↕️ | Sorts a Series or DataFrame by its values in descending order. |
| **`.head(n)`** | 🔝 | Displays the top `n` rows of the DataFrame or Series. |
| **`(boolean_series == value).sum()`** | ✅ | Used to count how many elements in a Series satisfy a certain condition (e.g., counting rows with zero missing values). |
