# Car Price Dataset Analysis

## Project Overview
This project uses Python and the Pandas library to analyze a car price dataset. It answers questions about car prices, brands, fuel types, mileage, transmission types, model years, engine sizes, doors, and ownership.

## Objectives
- Calculate the average price of cars.
- Identify the brand with the highest average price.
- Find the most common fuel type.
- Analyze mileage, transmission, and engine size.
- Compare prices across fuel types and years.
- Explore ownership counts and other car features.

## Technologies Used
- Python
- Pandas
- CSV dataset

## Dataset
The project uses a CSV file named car_price_dataset.csv.

## Questions Explored
1. What is the average price of all cars?
2. Which car brand has the highest average price?
3. What is the most common fuel type?
4. How many cars have mileage greater than 200,000?
5. What is the distribution of cars by transmission type?
6. Which car model has the highest price?
7. What is the average price of cars by fuel type?
8. How many cars are from the year 2020 or later?
9. What is the average engine size for each brand?
10. Which car has the lowest mileage?
11. What is the correlation between mileage and price?
12. How many cars have more than two owners?
13. What is the average price of cars by year?
14. What is the highest number of doors among the cars?
15. What is the average mileage for each fuel type?
16. How many cars are from the Toyota brand?
17. What is the average price of cars with automatic transmission?
18. Which car has the highest owner count?
19. What is the average engine size for diesel cars?
20. How many cars have a price greater than $10,000?

## How to Run
1. Install Python.
2. Install Pandas:
   ```bash
   pip install pandas
   ```
3. Place car_price_dataset.csv in the correct folder.
4. Open and run the Python file or notebook in Google Colab, Jupyter Notebook, or another compatible environment.

## Example Code
```python
import pandas as pd

df = pd.read_csv("car_price_dataset.csv")

# Average price of all cars
print(df["Price"].mean())

# Average price by brand
print(df.groupby("Brand")["Price"].mean())

# Most common fuel type
print(df["Fuel_Type"].value_counts().idxmax())
```

## Skills Practiced
- Loading CSV data with Pandas
- Selecting DataFrame columns
- Calculating averages with mean()
- Grouping data with groupby()
- Counting values with value_counts()
- Finding maximum and minimum values
- Filtering rows using conditions
- Exploring relationships between numerical columns

## Notes
Some calculations in the original code may need correction, including the year filter, owner-count maximum, and Boolean-condition counts. Question 11 (correlation) is listed but does not yet contain calculation code. Verify results before publishing.

## Author
Kavita Jadhav

## Purpose
Educational project for practicing Python and Pandas data analysis.
