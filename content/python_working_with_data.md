# 2 Data in Python
It is recommended that the Pandas library is used when working with data in Python.

## 2.1 Setting up Pandas
If Pandas is not already installed, it can be done so via the command line or an IDE console
```py
pip install pandas
```
or
```py
py -x.xx -m pip install pandas
# where x.xx is the Python version
```
To import the pandas library to use in code
```py
import pandas as pd
```
## 2.2 Extract data from an external file into a DataFrame
```py
df = pd.read_csv('./data/csv_file.csv')
```
## 2.3 View data in a dataframe
```py
print(df.head()) # Default is 5 rows
# Note that Pandas is 0 indexed, rows start at 0

print(df.head(3))
```
## 2.4 Extract data from a SQL database into a DataFrame
```py
import pandas as pd
import sqlite3

# Connect to the database
conn = sqlite3.connect('your_database.db')

# Query data into a DataFrame
query = "SELECT * FROM your_table_name"
df = pd.read_sql_query(query, conn)
# Replace 'your_database.db' with your database file and 'your_table_name' with your table name.
```
## 2.5 Limit the variables (columns) in your DataFrame
```py
# To keep specific columns
columns_to_keep = ['column1', 'column2']
df = df[columns_to_keep]

# To drop specific columns
columns_to_drop = ['column_to_drop1', 'column_to_drop2']
df = df.drop(columns=columns_to_drop)
```
## 2.6 Import just the top n rows
```py
# Specify the path to your CSV file
csv_file_path = 'your_file.csv'

# Use the 'read_csv' function to read the CSV file
# Use the 'nrows' parameter to specify the number of rows to read (in this case, 10)
df = pd.read_csv(csv_file_path, nrows=10)
```
## 2.7 Import specific columns
```py
# Specify the columns you want to read
columns_to_read = ['Column1', 'Column2', 'Column3']

# Read the CSV file with only the specified columns
df = pd.read_csv('your_file.csv', usecols=columns_to_read)
```
## 2.8 View data types of DataFrame columns
```py
# To see data types of all columns
print(df.dtypes)

# To get the data type of a specific column (e.g., 'column1')
print(df['column1'].dtype)
```
## 2.9 Combine tables vertically and horizontally
```py
# Vertical concatenation (stacking rows)
result_vertical = pd.concat([df1, df2])

# Horizontal concatenation (not join, appended horizontally)
result_horizontal = pd.concat([df1, df2], axis=1)
```
## 2.10 Perform left joins, right joins, and full joins
```py
# Left join
result_left = pd.merge(df1, df2, on='common_column', how='left')

# Right join
result_right = pd.merge(df1, df2, on='common_column', how='right')

# Full join (outer join)
result_full = pd.merge(df1, df2, on='common_column', how='outer')


# Join on multiple columns
df1 = pd.DataFrame({
    'key1': ['A', 'B', 'C', 'D'],
    'key2': ['X', 'Y', 'Z', 'W'],
    'value1': [1, 2, 3, 4]
})

df2 = pd.DataFrame({
    'key1': ['B', 'A', 'C', 'E'],
    'key2': ['Y', 'X', 'Z', 'V'],
    'value2': [5, 6, 7, 8]
})

# Join on multiple specific columns (key1 and key2)
result = pd.merge(df1, df2, on=['key1', 'key2'])
```
## 2.11 Output a DataFrame
```py
# To save the DataFrame to a CSV file
result.to_csv('output_file.csv', index=False)

# Replace 'output_file.csv' with the desired file name and path.

# index=False omits the row numbers from the output
```
