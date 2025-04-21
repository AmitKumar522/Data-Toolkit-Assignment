# 📊 Load CSV with Pandas - Python Data Handling

![Python + Pandas](https://media.giphy.com/media/KAq5w47R9rmTuvWOWa/giphy.gif)

## 🧠 Project Overview

This mini project demonstrates how to use **Pandas** in Python to:

✅ Create a sample CSV file  
✅ Load that CSV using `pandas.read_csv()`  
✅ Display the first 5 rows using `.head()`

It’s great for beginners exploring **data handling** and **CSV file manipulation** in Python! 🚀

---

## 💻 Technologies Used

- Python 🐍
- Pandas 📦
- CSV file format 📁

---

## 🧾 Sample Code

```python
import pandas as pd

# Sample data creation
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Eva', 'Frank'],
    'Age': [25, 30, 22, 35, 28, 26],
    'City': ['New York', 'Los Angeles', 'Chicago', 'Houston', 'Phoenix', 'Boston']
}
df = pd.DataFrame(data)
df.to_csv('people.csv', index=False)

# Reading the CSV
df_loaded = pd.read_csv('people.csv')

# Display first 5 rows
print(df_loaded.head())
