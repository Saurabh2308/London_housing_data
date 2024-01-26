# London_housing_data
Importing Libraries and Reading Data
Importing Libraries:

import pandas as pd: Imports the Pandas library and aliases it as pd.
Reading the Data:

df = pd.read_csv("file.csv"): Reads the dataset from a CSV file into a Pandas DataFrame named df.
Initial Data Exploration
Displaying Initial Data:

df.head(): Displays the first few rows of the DataFrame to provide a preview of the data.
Data Information:

df.info(): Provides information about the DataFrame, including column names, data types, and non-null counts.
df.count(): Returns the count of non-null values for each column.
Checking Null Values:

df.isna().sum().sort_values(ascending=False): Calculates the sum of null values for each column and sorts them in descending order.
Visualizing Null Values:

sns.heatmap(df.isna()): Creates a heatmap visualization to visualize null values in the DataFrame.
Data Preprocessing
Converting Date Column:

Converts the 'date' column from string to datetime format using pd.to_datetime().
Adding Year and Month Columns:

Extracts year and month from the 'date' column and adds them as separate columns to the DataFrame.
Data Analysis
Filtering and Analysis:
Filters records where the 'no_of_crimes' column is zero and displays the corresponding records.
Calculates and displays the maximum and minimum average price per year in England.
Calculates and displays the maximum and minimum number of crimes recorded per year.
Counts the total number of records for each area where the average price is less than 100,000.
Explanation
This code demonstrates various data analysis tasks using Pandas, including data loading, exploration, preprocessing, and analysis. It provides insights into housing prices, crime rates, and other related variables over time. The analysis helps in understanding trends, identifying outliers, and gaining insights into the dataset. Additionally, visualizations such as heatmaps can aid in identifying missing values in the dataset. Overall, this code showcases the power of Pandas for data analysis and manipulation tasks.
