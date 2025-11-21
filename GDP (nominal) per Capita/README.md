# 📊 Advanced Pandas Practice: GDP and MPG Data Analysis

This repository contains two Jupyter Notebooks (`Pandas Practice Notebook JennyGUO 17_Nov_1.ipynb` and `Regional Pandas Practice JennyGUO 17Nov-2.ipynb`) and two datasets (`GDP (nominal) per Capita.csv` and `mpg.csv`). The notebooks demonstrate essential steps in the data science workflow, including Data Cleaning, Exploratory Data Analysis (EDA), and Data Visualization.

***

## 📁 Data Sources & Structure

This project uses two distinct datasets to practice different aspects of Pandas manipulation.

### 💰 GDP (nominal) per Capita.csv

This dataset contains Gross Domestic Product (GDP) per capita estimates for various countries/territories, sourced from different international organizations (IMF, World Bank, UN).

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **`Country/Territory`** | Object (String) | The name of the country or territory. |
| **`UN_Region`** | Object (String) | The geographic region as defined by the UN. |
| **`IMF_Estimate`** | Numeric | GDP per capita estimate from the International Monetary Fund. |
| **`IMF_Year`** | Numeric | The year corresponding to the IMF estimate. |
| **`WorldBank_Estimate`** | Numeric | GDP per capita estimate from the World Bank. |
| **`WorldBank_Year`** | Numeric | The year corresponding to the World Bank estimate. |
| **`UN_Estimate`** | Numeric | GDP per capita estimate from the United Nations. |
| **`UN_Year`** | Numeric | The year corresponding to the UN estimate. |

### 🚗 mpg.csv

This well-known dataset contains information on fuel economy for 234 car models, which is typically used for practice in data filtering and correlation analysis.

| Column | Description |
| :--- | :--- |
| `manufacturer` | Car manufacturer (e.g., Audi, Ford) |
| `model` | Specific model name |
| `displ` | Engine displacement in litres |
| `year` | Model year (1999 or 2008) |
| `cyl` | Number of cylinders |
| `trans` | Type of transmission (e.g., auto, manual) |
| `drv` | Drive type: front-wheel (**f**), rear-wheel (**r**), or 4-wheel (**4**) |
| `cty` | City miles per gallon (MPG) |
| `hwy` | Highway MPG |
| `fl` | Fuel type |
| `class` | Vehicle class (e.g., compact, SUV) |

***

## 📚 Notebook Analysis Scope

The two Python files cover a comprehensive data analysis pipeline:

1.  **Exploratory Data Analysis (EDA) & Summary Statistics:** Using functions like `head()`, `info()`, and `describe()` to understand data distributions and quality.
2.  **Handling Missing Data:** Identifying, counting, and imputing/filling null values using various Pandas techniques.
3.  **Outlier Detection & Removal:** Employing statistical and visual methods to detect and handle extreme values that could skew analysis.
4.  **Regional Aggregation:** Using **Group By** operations to calculate statistics (like mean, median) for different geographical regions (`UN_Region`).
5.  **Data Visualization:** Creating charts (using Matplotlib/Seaborn, as mentioned in the notebooks) to explore patterns and communicate insights.

***

## 🐍 Key Python Functions Used

The notebooks leverage the **Pandas** library (imported as `pd`) for data manipulation, cleaning, and analysis.

### 📥 Data Inspection & EDA

| Function/Attribute | Icon | Purpose |
| :--- | :--- | :--- |
| **`pd.read_csv('...')`** | 📂 | Loads data from a CSV file into a DataFrame. |
| **`df.info()`** | ℹ️ | Prints a summary of the DataFrame (data types, non-null counts). |
| **`df.describe()`** | 📈 | Generates descriptive statistics (count, mean, std, min, max, quartiles) for numeric columns. |
| **`df.head()` / `df.tail()`** | 🔝 | Displays the first or last few rows of the DataFrame. |
| **`df.corr()`** | 📉 | Calculates the pairwise correlation between all numeric columns. |

### 🧼 Data Cleaning & Missing Values

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`df.isna()`** | 🤔 | Returns a Boolean DataFrame/Series indicating where values are missing (`True`). |
| **`df.isna().sum()`** | ➕ | Counts the total number of missing values per column. |
| **`df.fillna(value)`** | 🔄 | Replaces missing values (`NaN`) with a specified value (e.g., median, mean, or 0). |
| **`df.dropna()`** | ✂️ | Removes rows or columns that contain missing values. |
| **`df['col'].replace(...)`** | ✍️ | Replaces specific values within a column (e.g., replacing text or outlier values). |

### 🔢 Grouping & Aggregation

| Function/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`df.groupby('col')`** |  groupBy | Groups the DataFrame using one or more columns, preparing for aggregation. |
| **`.mean()` / `.median()`** | 🔢 | Calculates the average or middle value within each group. |
| **`.count()`** | #️⃣ | Counts the number of non-null values within each group. |
| **`df[mask]`** | 🎯 | Filters rows using a Boolean condition for subset analysis. |

### 🖼️ Visualization

| Library/Method | Icon | Purpose |
| :--- | :--- | :--- |
| **`import matplotlib.pyplot as plt`** | 🖼️ | The primary library for creating static, interactive, and animated visualizations in Python. |
| **`import seaborn as sns`** | 🎨 | A high-level data visualization library based on Matplotlib, providing attractive statistical graphics. |
