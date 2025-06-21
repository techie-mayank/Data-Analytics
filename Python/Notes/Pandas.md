# 🐼 Pandas Essentials

> Pandas is a powerful Python library for data manipulation, analysis, and cleaning. It provides DataFrame and Series data structures built on top of NumPy.

---

## 📦 1. Installation
```bash
pip install pandas
```

---

## 🧠 2. Key Data Structures

| Structure | Description                         |
|----------|-------------------------------------|
| Series   | 1D labeled array                     |
| DataFrame | 2D labeled table (rows + columns)  |

```python
import pandas as pd

s = pd.Series([1, 2, 3])
df = pd.DataFrame({'A': [1, 2], 'B': [3, 4]})
```

---

## 📂 3. Data Input & Output

```python
pd.read_csv('file.csv')           # Read CSV
pd.read_excel('file.xlsx')        # Read Excel
df.to_csv('output.csv')           # Write CSV
df.to_excel('output.xlsx')        # Write Excel
```

---

## 🔍 4. Exploring Data

```python
df.head()                         # First 5 rows
df.tail(3)                        # Last 3 rows
df.shape                          # (rows, columns)
df.info()                         # Summary info
df.describe()                     # Stats summary
df.columns                        # Column names
df.index                          # Row indices
df.dtypes                         # Data types
```

---

## 🧮 5. Selecting Data

```python
df['column_name']                 # Single column
df[['col1', 'col2']]              # Multiple columns
df.loc[0]                         # Row by label/index
df.iloc[0]                        # Row by position
df.loc[0, 'col1']                 # Specific value
df.iloc[0, 1]                     # Value by position
```

---

## 🔁 6. Filtering and Boolean Indexing

```python
df[df['col1'] > 5]
df[(df['col1'] > 5) & (df['col2'] < 10)]
df[df['col'].isin(['A', 'B'])]
```

---

## 🧹 7. Cleaning Data

```python
df.dropna()                       # Remove missing
df.fillna(0)                      # Replace missing
df.replace('?', np.nan)          # Replace values
df.rename(columns={'A': 'a'})     # Rename columns
df.drop(columns=['col'])          # Drop column
df.duplicated().sum()             # Count duplicates
```

---

## 🧱 8. Data Transformation

```python
df['col'] = df['col'].astype(int)     # Change type
df['new'] = df['col1'] + df['col2']   # Create column
df.apply(np.sqrt)                     # Apply function
df['col'].map({'A': 1, 'B': 2})       # Map values
```

---

## 🧮 9. Aggregation and Grouping

```python
df.groupby('col').mean()          # Grouped mean
df.groupby(['col1', 'col2']).sum()
df['col'].value_counts()          # Frequency counts
```

---

## 📊 10. Sorting

```python
df.sort_values(by='col', ascending=False)
df.sort_index()
```

---

## 📐 11. Merging & Joining

```python
pd.concat([df1, df2])             # Append rows
pd.concat([df1, df2], axis=1)     # Append columns
pd.merge(df1, df2, on='key')      # Merge on key
pd.merge(df1, df2, how='left')    # Left join
```

---

## 🔄 12. Pivot Tables

```python
df.pivot_table(index='A', columns='B', values='C', aggfunc='sum')
```

---

## 🕵️ 13. Date & Time

```python
pd.to_datetime(df['date'])        # Convert to datetime
df['date'].dt.year                # Extract year
df['date'].dt.month_name()       # Month name
df.set_index('date')             # Set date index
```

---

## 📘 14. Recommended Practice

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Pandas Exercises on W3Resource](https://www.w3resource.com/python-exercises/pandas/)
