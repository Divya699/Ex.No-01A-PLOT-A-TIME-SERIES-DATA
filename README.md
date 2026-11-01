# Ex.No: 01A PLOT A TIME SERIES DATA

##  Date: 01/11/2026
## NAME : DIVYA PRIYA S
##  REGISTER NO: 212225240037

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# SOFTWARE REQUIRED 

1 . Jupyter Notebook

# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
from matplotlib import pyplot as plt
import pandas as pd

# Read the canteen dataset
df = pd.read_csv("canteen_shop_data.csv)

# Convert Date into datetime format
df['Date'] = pd.to_datetime(df['Date'])

# Convert Employee ID into numeric
df['Employee ID'] = pd.to_numeric(df['Employee ID'])

# Plot Date vs Employee ID
plt.plot(df['Date'], df['Employee ID'], color='black')

# Title and labels
plt.title('Time Series Plot of Employee ID by Date')
plt.xlabel('Date')
plt.ylabel('Employee ID')

# Grid
plt.grid(True)

# Show graph
plt.show()
```


# OUTPUT:

<img width="674" height="528" alt="image" src="https://github.com/user-attachments/assets/1a5b06ae-d915-4dfc-aeb0-ad07a08f30db" />





# RESULT:
Thus we have created the python code for plotting the time series of given data.
