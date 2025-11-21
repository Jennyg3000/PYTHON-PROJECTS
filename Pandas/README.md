# 📖 Pandas DataFrame Basics

This repository contains a Jupyter Notebook (`PandasDataFrames_Day4_01 JennyGuo.ipynb`) demonstrating the fundamental operations and properties of **Pandas DataFrames** in Python. It covers the initial steps of data manipulation and inspection crucial for any data analysis project.

***

## 🚀 Project Objectives

The notebook addresses the following core functionalities of the Pandas library:

* **Creation:** Making DataFrames from various Python collections (e.g., lists of dictionaries).
* **Inspection:** Understanding a DataFrame's properties and basic information.
* **Selection:** Accessing and selecting single columns (Series).
* **Modification:** Adding new columns and renaming existing ones.
* **Analysis:** Generating descriptive statistics for numeric columns.
* **Export:** Saving the final DataFrame to a CSV file.

***

## 🐍 Key Python Functions Used

The notebook utilizes the following key functions and attributes from the **Pandas** library (imported as `pd`):

### 🛠️ DataFrame Creation and Inspection

| Function/Attribute | Icon | Purpose |
| :--- | :--- | :--- |
| **`import pandas as pd`** | 🐼 | Imports the pandas library. |
| **`pd.DataFrame(...)`** | 🏗️ | Constructs a DataFrame from Python data structures. |
| **`df.shape`** | 📐 | Returns a tuple representing the dimensions (`(rows, columns)`) of the DataFrame. |
| **`df.index`** | 🏷️ | Displays the index (row labels) of the DataFrame. |
| **`df.columns`** | 📋 | Displays the column labels of the DataFrame. |
| **`df.info()`** | ℹ️ | Prints a concise summary, including data types and non-null values. |
| **`df.head(n)`** | 🔝 | Returns the first `n` rows. |

### ➡️ Column Selection and Modification

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`df['column_name']`** | 🎯 | Selects and returns a single column as a Pandas Series. |
| **`df['new_col'] = value`** | ✨ | Adds a new column to the DataFrame, assigning a fixed value or a calculated Series to all rows. |
| **`df.rename(columns={'old':'new'}, inplace=True)`** | ✍️ | Renames specified columns in the DataFrame. |
| **`df['col'].round(0).astype(int)`** | 🔄 | Chains methods to round numeric column values to the nearest whole number and convert the data type to integer. |

### 📈 Descriptive Statistics and Analysis

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`df['column'].describe()`** | 📊 | Generates descriptive statistics (count, mean, std, min, max, quartiles) for a numeric column. |
| **`df['column'].sum()`** | ➕ | Calculates the sum of values in the column. |
| **`df['column'].min()`** | ⬇️ | Finds the minimum value in the column. |
| **`df['column'].max()`** | ⬆️ | Finds the maximum value in the column. |

### 📤 Data Export

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`df.to_csv('output.csv', index=False)`** | 💾 | Exports the DataFrame data to a CSV file, excluding the DataFrame's index. |

***

## 💡 How to Run the Notebook

1.  Clone this repository.
2.  Ensure you have **Python** and the **Pandas** library installed.
    ```bash
    pip install pandas jupyter
    ```
3.  Open the file in Jupyter environment:
    ```bash
    jupyter notebook "PandasDataFrames_Day4_01 JennyGuo.ipynb"
    ```
4.  Run the cells sequentially to see the creation and transformation of the sample DataFrame.
