Road Traffic Accident Analysis
This script analyzes road traffic accident data to understand the influence of road surface conditions, weather conditions, and time of day on the number of accidents. The analysis includes data cleaning, descriptive statistics, correlation analysis, and visualization.

Prerequisites:
->Python 3.x
->Pandas library
->Seaborn library
->Matplotlib library

Script:
#Task-5
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the data
   # Update this with your actual file path
df = pd.read_csv("C:\dbms\RTA Dataset.csv")

# Data Cleaning
df.dropna(subset=['Road_surface_conditions', 'Weather_conditions', 'Time'], inplace=True)
df['Time'] = pd.to_datetime(df['Time'], format='%H:%M:%S').dt.hour

# Descriptive Statistics
descriptive_stats = df[['Road_surface_conditions', 'Weather_conditions', 'Time']].describe()
print("Descriptive Statistics:\n", descriptive_stats)

# Correlation Analysis
correlation = df[['Road_surface_conditions', 'Weather_conditions', 'Time']].apply(lambda x: pd.factorize(x)[0]).corr()
print("\nCorrelation Analysis:\n", correlation)

# Visualization

# Bar chart for accidents by road condition
plt.figure(figsize=(10, 6))
sns.countplot(x='Road_surface_conditions', data=df)
plt.title('Accidents by Road Condition')
plt.xlabel('Road Condition')
plt.ylabel('Number of Accidents')
plt.xticks(rotation=45)
plt.show()

# Bar chart for accidents by weather condition
plt.figure(figsize=(10, 6))
sns.countplot(x='Weather_conditions', data=df)
plt.title('Accidents by Weather Condition')
plt.xlabel('Weather Condition')
plt.ylabel('Number of Accidents')
plt.xticks(rotation=45)
plt.show()

# Line chart for accidents by time of day
plt.figure(figsize=(10, 6))
sns.countplot(x='Time', data=df)
plt.title('Accidents by Time of Day')
plt.xlabel('Hour of Day')
plt.ylabel('Number of Accidents')
plt.show()

Description:
This script performs the following tasks:

Import Libraries:

Imports necessary libraries for data processing (pandas), visualization (seaborn, matplotlib).
Load Data:

Loads the road traffic accident dataset from the specified file path.
Data Cleaning:

Removes rows with missing values in 'Road_surface_conditions', 'Weather_conditions', and 'Time' columns.
Converts the 'Time' column to represent the hour of the day.
Descriptive Statistics:

Computes and prints descriptive statistics for 'Road_surface_conditions', 'Weather_conditions', and 'Time'.
Correlation Analysis:

Factorizes categorical variables and calculates the correlation matrix, which is printed to the console.
Visualization:

Creates bar charts to show the number of accidents by road surface condition and weather condition.
Creates a line chart to show the number of accidents by the hour of the day.

Output:
Running this script will output descriptive statistics, a correlation matrix, and visualizations including:

Bar Chart: Number of accidents by road surface condition.
Bar Chart: Number of accidents by weather condition.
Line Chart: Number of accidents by time of day.

![des](https://github.com/Lavanya-1234198/PRODIGY_DS_05/assets/174336088/3de6c765-1d0b-4306-ae59-ecb9f91b4af6)

![g1](https://github.com/Lavanya-1234198/PRODIGY_DS_05/assets/174336088/adab54f2-113d-42fb-bd5a-e6077136cf0c)

![g2](https://github.com/Lavanya-1234198/PRODIGY_DS_05/assets/174336088/e68d9f76-fd32-40fd-87b3-a9162bb86c63)

![g3](https://github.com/Lavanya-1234198/PRODIGY_DS_05/assets/174336088/91b4580d-e791-4b16-89ca-d684ccc0fab4)
