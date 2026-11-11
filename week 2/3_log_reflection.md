This was the code AI provided: 

import pandas as pd

df = pd.read_csv("teaching_prices_messy.csv")

# Check the structure and missing values 
print(df.info())  (KEEP)

print(df.isnull().sum()) (MODIFY - IN CLASS WE WERE TAUGHT df.isna)

# Remove completely duplicated rows
df = df.drop_duplicates()  (KEEP)

# Remove a duplicated column if it has the same values as another column
df = df.loc[:, ~df.columns.duplicated()]  (REJECT)

# Convert date to datetime
df["date"] = pd.to_datetime(df["date"], errors="coerce")  (REJECT)

# Convert price to numeric
df["price"] = pd.to_numeric(df["price"], errors="coerce")  (KEEP)

# Fill missing price with the median price
df["price"] = df["price"].fillna(df["price"].median())  (REJECT)

# Check the cleaned data  (KEEP)
print(df.info())

print(df.isnull().sum())


REFLECT: My main decision differed from the AI's suggestion for the missing price. The AI suggested replacing it with the median, whereas I would retain or flag the missing value because there is not enough evidence to know its true value. My decision is better supported because it avoids inventing information that was not present in the original dataset.
