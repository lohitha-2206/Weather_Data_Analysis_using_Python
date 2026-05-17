# 🌦️ Weather Data Analysis using Python & Pandas

## 📌 Project Introduction

This project is based on performing data analysis and preprocessing operations on a Weather Dataset using Python and the Pandas library inside Jupyter Notebook. The dataset contains weather-related information such as Temperature, Humidity, Wind Speed, Visibility, Pressure, and Weather Conditions.

The main objective of this project is to understand how Python and Pandas are used in real-world weather data analysis for cleaning, exploring, filtering, and analyzing structured datasets efficiently.

In this project, different data analysis techniques were implemented such as:

- Data Cleaning
- Handling Missing Values
- Data Filtering
- Statistical Analysis
- GroupBy Operations
- Weather Condition Analysis
- Exploratory Data Analysis (EDA)

This project provides practical exposure to working with weather datasets and understanding how data analysts use Python for extracting meaningful insights from real-world data.

---

# 📂 Dataset Information

The dataset contains weather observations and atmospheric conditions recorded at different times.

### Dataset Features:

- Date/Time
- Temperature
- Dew Point Temperature
- Relative Humidity
- Wind Speed
- Visibility
- Pressure
- Weather Condition

Each record in the dataset represents a specific weather observation.

---

# 🛠️ Tools & Technologies Used

## 🐍 Python
Python was used as the programming language for performing data analysis and dataframe operations.

## 📊 Pandas
Pandas library was used for:
- Data Cleaning
- Data Manipulation
- Handling Missing Values
- Filtering Data
- Statistical Analysis
- GroupBy Operations

## 📓 Jupyter Notebook
Jupyter Notebook was used to execute Python code interactively and visualize outputs step-by-step.

---

# 🔍 Pandas Functions Implemented

## 🔹 import pandas as pd
Used to import the Pandas library.

### Syntax:
```python
import pandas as pd
```

---

## 🔹 pd.read_csv()
Used to import the CSV dataset into Jupyter Notebook.

### Syntax:
```python
data = pd.read_csv("Weather_Data.csv")
```

---

## 🔹 head()
Displays the first 5 rows of the dataset.

### Syntax:
```python
data.head()
```

---

## 🔹 shape
Shows the total number of rows and columns in the dataset.

### Syntax:
```python
data.shape
```

---

## 🔹 columns
Displays the names of all columns.

### Syntax:
```python
data.columns
```

---

## 🔹 dtypes
Shows the datatype of each column.

### Syntax:
```python
data.dtypes
```

---

## 🔹 unique()
Displays unique values from a column.

### Syntax:
```python
data['Wind Speed_km/h'].unique()
```

---

## 🔹 nunique()
Shows the total number of unique values.

### Syntax:
```python
data.nunique()
```

---

## 🔹 value_counts()
Displays unique values along with their occurrence count.

### Syntax:
```python
data['Weather'].value_counts()
```

---

## 🔹 isnull().sum()
Detects missing/null values from each column.

### Syntax:
```python
data.isnull().sum()
```

---

## 🔹 groupby()
Groups data according to a specific column.

### Syntax:
```python
data.groupby('Weather Condition').mean(numeric_only=True)
```

---

# 📊 Tasks Performed in the Project

## ✅ Q1) Finding Unique Wind Speed Values

### Task:
Find all the unique Wind Speed values in the dataset.

### Code Used:
```python
data['Wind Speed_km/h'].unique()
```

### Explanation:
- Displays all unique wind speed values
- Helps understand different wind speed variations in the dataset

---

# 📊 Q2) Counting Clear Weather Conditions

### Task:
Find the number of times when Weather is exactly Clear.

### Code Used:
```python
data[data['Weather'] == 'Clear']
```

### Explanation:
- Filters records where weather condition is Clear
- Helps analyze frequency of clear weather

---

# 📊 Q3) Handling Null Values

### Task:
Find all the null values in the dataset.

### Code Used:
```python
data.isnull().sum()
```

### Explanation:
- Detects missing values from each column
- Important for data cleaning and preprocessing

---

# 📊 Q4) Statistical Analysis

### Task:
Find Mean Visibility, Standard Deviation of Pressure, and Variance of Relative Humidity.

### Code Used:
```python
data.Visibility_km.mean()

data.Press_kPa.std()

data['Rel Hum_%'].var()
```

### Explanation:
- Mean helps identify average visibility
- Standard deviation measures pressure variation
- Variance shows humidity data spread

---

# 📊 Q5) GroupBy Weather Condition

### Task:
Find mean values of each column against each Weather Condition.

### Code Used:
```python
data.groupby('Weather Condition').mean(numeric_only=True)
```

### Explanation:
- Groups data based on weather conditions
- Calculates average values for numeric columns
- Useful for comparative weather analysis

---

# 📊 Q6) Filtering Records using Conditions

### Task:
Find all instances where Weather is Clear or Visibility is above 40.

### Code Used:
```python
data[(data['Weather Condition'] == 'Clear') | (data['Visibility_km'] > 40)]
```

### Explanation:
- Uses conditional filtering
- Displays records matching either condition
- Helps in advanced weather analysis

---

# 📌 Important Insights

✔️ Pandas makes weather data analysis simple and efficient.

✔️ GroupBy operations help compare different weather conditions.

✔️ Statistical analysis helps understand weather trends and variations.

✔️ Filtering records allows targeted weather analysis.

✔️ Missing values can be detected easily using Pandas functions.

✔️ Real-world datasets can be analyzed efficiently using Python.

---

# 📁 Project Structure

```text
├── Weather_Data_Analysis.ipynb
├── Weather_Data.csv
├── README.md
```

---

# 🎯 Final Conclusion

This project demonstrates how Python and Pandas can be used for real-world weather data analysis and preprocessing tasks. Different operations such as handling null values, filtering records, statistical analysis, grouping data, and extracting meaningful insights were successfully implemented.

Through this project, practical understanding was gained in:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Manipulation using Pandas
- Statistical Analysis
- GroupBy Operations
- Python-based Data Analytics

Overall, this project serves as a strong beginner-friendly foundation for learning Data Analysis and Data Science using Python.
