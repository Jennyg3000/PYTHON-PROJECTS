# Python Fundamentals & Pandas Data Analysis Repository 🐍📊

This repository contains a series of Jupyter Notebook exercises designed to build a solid **Python programming foundation** and introduce the core concepts of data processing using the **Pandas** library.

---

## 📁 Repository File Structure

| File Name | Description | Core Topics |
| :--- | :--- | :--- |
| `Python Day 1 Exercises JennyGUO.ipynb` | **Python Basics**: Variables, data types, basic arithmetic operations, and user input/output. | Basic Syntax & I/O |
| `Python Day 2_Task 1 Exercises JennyGuo.ipynb` | **Python Control Flow**: Conditional statements (`if/elif/else`) and iterative structures (`for`/`while` loops). | Logic Control & Iteration |
| `Pandas Day1.ipynb` | **Pandas Introduction**: Data importing (`.csv`), DataFrame structure, and fundamental data viewing operations. | Data Processing |
| `student.xlsx - in.csv` | The raw data file used for Pandas exercises (includes student ID, name, class, mark, and gender information). | Raw Data Source |

---

## 🐍 Python Fundamentals & Control Flow 

This section focuses on mastering the building blocks of Python programming, including user interaction and controlling program logic.

### 1. Basic Functions and Type Conversion ⚙️

| Function/Concept | Description | Example Usage (from files) | Reference File |
| :--- | :--- | :--- | :--- |
| **`input()`** | Retrieves data from the console as a **string** type, enabling user interaction. | Getting name, age, or a multi-digit number | `Python Day 1...` |
| **`print()`** | Outputs messages to the console, often combined with f-strings for formatted output. | Displaying greetings and calculation results | `Python Day 1...` |
| **`int()` / `str()`** | **Data Type Conversion** functions: Used to convert input into an **integer** (`int`) or convert numbers back to a **string** (`str`). | Ensuring numbers are treated numerically for calculations | `Python Day 1...` |
| **f-string** | Formatted String Literals (`f"..."`), used to embed expressions and variables directly within a string. | Printing factorial results clearly | `Pandas Day1.ipynb` |

### 2. Control Flow Structures 🧭

| Structure/Operator | Description | Example Usage (from files) | Reference File |
| :--- | :--- | :--- | :--- |
| **`if / elif / else`** | **Conditional Statements**: Executes different blocks of code based on whether a boolean expression is `True` or `False`. | Building basic security door access logic | `Python Day 2...` |
| **`while` loop** | **Conditional Loop**: Repeats a block of code **while** a specific condition remains `True`, ideal for unknown iteration counts. | Repeatedly prompting for a password until it's correct | `Python Day 2...` |
| **`for` loop & `range()`** | **Iterative Loop**: Used to iterate over a sequence. `range()` is commonly used to iterate a specific number of times. | Calculating the factorial of a number | `Pandas Day1.ipynb` |
| **`//` (Floor Division) & `%` (Modulus)** | **Arithmetic Operators**: Key for integer division and finding the remainder, crucial for extracting or reversing digits. | Extracting the thousands, hundreds, tens, and units digits from a 4-digit number | `Python Day 1...` |

---

## 📊 Pandas Data Analysis Introduction 

This section covers the essential first steps in data analysis: loading and structuring external data using the powerful Pandas library.

### Core Pandas Functions and Concepts 💡

| Function/Concept | Description | Reference File |
| :--- | :--- | :--- |
| **`import pandas as pd`** | Imports the **Pandas** library, aliasing it as `pd`. This is the standard practice for starting data analysis in Python. | `Pandas Day1.ipynb` |
| **`pd.read_csv()`** | The function used to read data from a CSV file (`student.xlsx - in.csv`) and load it into a DataFrame. | `Pandas Day1.ipynb` |
| **DataFrame** | The fundamental Pandas data structure, which organizes data in a two-dimensional labeled structure (rows and columns), similar to an Excel sheet or SQL table. | Storing student data (ID, Name, Mark, Gender) | `Pandas Day1.ipynb` |
