# Hamza-final-project-pf

# README for Healthcare Dataset Analysis Notebook

## Overview
This Jupyter Notebook provides a comprehensive analysis of the `healthcare-dataset-stroke-data.csv` dataset. It focuses on exploring the dataset, understanding its structure, and extracting insights through statistical summaries and data selection operations.

## Requirements

### Python Version
- Python 3.x

### Dependencies
To run this notebook, ensure the following libraries are installed:

- pandas

You can install the required library using pip:
```bash
pip install pandas
```

## Dataset
The notebook works with the `healthcare-dataset-stroke-data.csv` file. Ensure the file is in the same directory as the notebook or adjust the file path accordingly.

## Code Explanation
Below is a detailed explanation of the notebook code:

### 1. Importing Libraries
```python
import pandas as pd
```
This line imports the pandas library, which is used for data manipulation and analysis.

### 2. Loading the Dataset
```python
df = pd.read_csv("healthcare-dataset-stroke-data.csv")
```
This reads the CSV file into a pandas DataFrame named `df`.

### 3. Exploring the Dataset

#### Display the Dataset
```python
df
```
Shows the entire dataset.

#### Display First 4 Rows
```python
df.head(4)
```
Displays the first 4 rows of the dataset.

#### Display Last 4 Rows
```python
df.tail(4)
```
Displays the last 4 rows of the dataset.

#### Display a Random Row
```python
df.sample()
```
Displays a random row from the dataset.

### 4. Dataset Properties

#### Shape of the Dataset
```python
df.shape
```
Returns the number of rows and columns in the dataset.

#### Size of the Dataset
```python
df.size
```
Returns the total number of elements in the dataset.

#### Data Types of Each Column
```python
df.dtypes
```
Displays the data types of each column in the DataFrame.

#### Dataset Values
```python
df.values
```
Returns the underlying data as a NumPy array.

#### Dataset Information
```python
df.info()
```
Provides a summary of the dataset, including the number of non-null values and data types of each column.

#### Index Information
```python
df.index
```
Displays the index (row labels) of the DataFrame.

#### Statistical Summary
```python
df.describe(include="all")
```
Generates descriptive statistics for numerical and categorical columns.

#### Column Names
```python
df.columns
```
Displays the names of all columns in the dataset.

### 5. Accessing Data

#### Select Single Column
```python
df["age"]
```
Returns the values of the `age` column.

#### Select Multiple Columns
```python
df[["gender", "age"]]
```
Returns the values of the `gender` and `age` columns.

#### Select Column Using Dot Notation
```python
df.id
```
Returns the values of the `id` column.

#### Select a Specific Row
```python
df.loc[2]
```
Returns the row with index 2.

#### Select a Range of Rows
```python
df.loc[35:40]
```
Returns rows with indices from 35 to 40.


