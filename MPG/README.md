# 🚗 Data Filtering and Analysis with Pandas: The MPG Dataset

This repository contains a Jupyter Notebook (`PandasDataFrames_02 JennyGuo.ipynb`) that focuses on essential **Pandas** techniques for selecting, filtering, and analyzing data using the `mpg.csv` dataset.

***

## 🚀 Project Objectives

This notebook is designed to teach and demonstrate the following core data manipulation concepts in Pandas:

* [cite_start]**Importing a CSV dataset**[cite: 1, 2].
* [cite_start]**Selecting multiple columns** from a DataFrame[cite: 1, 2].
* [cite_start]**Filtering rows** using **Boolean masks**[cite: 1, 2].
* [cite_start]Applying **AND (`&`) and OR (`|`) operators** for complex conditional filtering[cite: 1, 2].
* [cite_start]Understanding the proper use of the **`.copy()`** method[cite: 1, 2].
* [cite_start]**Sorting a DataFrame** by one or more columns[cite: 1, 2].
* [cite_start]**Counting True values** in a Boolean series[cite: 1, 2].
* Calculating column **correlation** (`.corr()`).

***

## ⛽ Data Source: `mpg.csv`

[cite_start]The data used, `mpg.csv` (Miles Per Gallon), contains 234 observations about various car models, their characteristics, and primarily their fuel economy[cite: 3, 4].

### 📝 Dataset Schema

| Column | Description |
| :--- | :--- |
| `manufacturer` | [cite_start]Car manufacturer (e.g., Audi, Ford, Toyota) [cite: 3, 4] |
| `model` | [cite_start]Specific model name [cite: 3, 4] |
| `displ` | [cite_start]Engine displacement in litres (numeric) [cite: 3, 4] |
| `year` | Year of the model (1999 or 2008) |
| `cyl` | [cite_start]Number of cylinders in the engine [cite: 3, 4] |
| `trans` | [cite_start]Type of transmission (e.g., automatic, manual) [cite: 3, 4] |
| `drv` | [cite_start]Drive type: front-wheel (**f**), rear-wheel (**r**), or 4-wheel (**4**) [cite: 3, 4] |
| `cty` | [cite_start]City miles per gallon (MPG) [cite: 3, 4] |
| `hwy` | [cite_start]Highway MPG [cite: 3, 4] |
| `fl` | [cite_start]Fuel type (e.g., **p**=premium, **r**=regular, **d**=diesel) [cite: 3, 4] |
| `class` | [cite_start]Vehicle class (e.g., compact, SUV, pickup) [cite: 3, 4] |

***

## 🐍 Key Pandas Methods Used

### 🔍 Selection and Filtering

| Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`pd.read_csv()`** | 📂 | [cite_start]Imports the dataset into a DataFrame[cite: 1, 2]. |
| **`df[['col1', 'col2']]`** | 🎯 | [cite_start]Selects multiple columns from the DataFrame[cite: 1, 2]. |
| **`df[mask]`** | 😷 | [cite_start]Filters rows based on a Boolean condition (mask)[cite: 1, 2]. |
| **`&` and `|`** | 🔗 | [cite_start]Combines multiple conditions using **AND** (`&`) or **OR** (`|`)[cite: 1, 2]. |
| **`.sum()`** | ✅ | [cite_start]Used on a Boolean Series (mask) to count the number of `True` values[cite: 1, 2]. |

### 📊 Aggregation and Sorting

| Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`.sort_values('col_name')`** | ↕️ | [cite_start]Sorts the DataFrame rows by values in a specified column[cite: 1, 2]. |
| **`.value_counts()`** | 🔢 | Displays unique values in a Series and counts their occurrences. |
| **`.corr()`** | 📉 | Calculates the correlation between columns in a DataFrame. |

### 💡 Best Practice

| Concept | Icon | Purpose |
| :--- | :--- | :--- |
| **`.copy()`** | 📝 | [cite_start]Creates a true, independent copy of a DataFrame subset to prevent unexpected side effects when modifying data[cite: 1, 2]. |
