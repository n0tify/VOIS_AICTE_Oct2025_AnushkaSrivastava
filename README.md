🏙️ Airbnb Open Data Exploratory Data Analysis (EDA)
📌 Project Overview
This project provides an in-depth Exploratory Data Analysis (EDA) and visualization of the Airbnb Open Data. The core objective is to uncover key market trends, identify pricing anomalies, and analyze property distribution across various geographical and listing types using clear, impactful visualizations built with Pandas, Matplotlib, and Seaborn.
💾 Data Source

File Name: 1730285881-Airbnb_Open_Data.xlsx - in.csv (or the discovered filename by the script)
Description: A public dataset containing detailed information on Airbnb listings, including pricing, host details, location coordinates, and review statistics.


⚙️ Setup and Execution
Prerequisites
To run the accompanying Jupyter Notebook, ensure you have a Python environment and the following libraries installed:
pip install pandas numpy matplotlib seaborn openpyxl

Running the Notebook

Placement: Ensure the data file is placed in the same directory as the Jupyter Notebook file.
Execution: Run the cells sequentially. The first cell is designed for automatic file discovery and will handle data loading and cleaning robustly.

🧼 Data Cleaning & Preparation
The initial code cell performs robust data cleaning to ensure data quality:

Robust Loading: Uses Python to automatically detect and load the file, suppressing the DtypeWarning.
Column Standardization: Converts all column names to lowercase and replaces spaces with underscores.
Price Cleaning: Converts the price column to a numeric type, removing currency symbols ($, ,) and handling outliers.
Outlier Handling: Filters out listings with prices of zero and extreme outliers (above the 99th percentile).
Missing Value Imputation: Fills missing values in critical columns like neighbourhood_group, neighbourhood, and number_of_reviews with 'Unknown' or 0.

✨ Key Visualization Objectives
The analysis is structured around the five specific business questions addressed in the visualizations:



Objective
Visualization Type
Insight Delivered



1. Count of Host per Listing
Bar Plot
Identifies the Top 10 Commercial Hosts (highest number of properties).


2. Top 10 Listings by Number of Reviews
Bar Plot
Highlights the most popular or frequently booked listings.


3. Neighbourhood Group vs. Price
Box Plot
Compares the overall price distribution and variance across major boroughs/groups.


4. Neighbourhood vs. Price (Top 10)
Bar Plot
Reveals the specific neighbourhoods with the highest average listing prices.


5. Room Type vs. Price
Violin Plot
Illustrates the full price distribution density comparing Entire Homes, Private Rooms, etc.

