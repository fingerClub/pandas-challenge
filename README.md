# pandas-challenge
the following was taken from chatGPT:
unique_values = df['my_column'].unique()

import pandas as pd

# Example DataFrame
data = {'Category': ['A', 'B', 'A', 'B'], 'Values': [10, 20, 30, 40]}
df = pd.DataFrame(data)

# Grouping the DataFrame by the 'Category' column
grouped = df.groupby('Category')

# Now 'grouped' is a DataFrameGroupBy object

# Example: Calculating the mean of each group
mean_values = grouped.mean()
print(mean_values)
# Compute the average math score by school for each grade, without setting 'school_name' as index
avg9 = df[df['grade'] == '9th'].groupby('school_name', as_index=False).mean()
