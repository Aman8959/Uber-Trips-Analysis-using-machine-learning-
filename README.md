# 🚕 Uber Trips Analysis

This project performs an exploratory data analysis (EDA) of Uber trip
data using Python and Pandas. The analysis focuses on understanding how
Uber ride demand varies by **day of the month, weekday, hour, and
geographical location**.

## 📌 Project Overview

The goal of this project is to explore Uber trip patterns and identify
useful insights from the available trip records.

The analysis follows these main steps:

1.  Import the required Python libraries
2.  Load the Uber trips dataset using Pandas
3.  Explore the dataset structure and properties
4.  Convert and extract useful date/time features
5.  Visualize trip density across different dimensions
6.  Draw observations from the visualizations

## 🗂️ Dataset

The notebook uses the following CSV file:

``` text
uber-raw-data-sep14.csv
```

The dataset contains Uber trip records for **September 2014** and
includes fields used for time-based and geographical analysis.

The notebook works with the following original columns:

-   `Date/Time` -- Date and time of the trip
-   `Lat` -- Latitude of the trip
-   `Lon` -- Longitude of the trip

Additional features are derived from `Date/Time`:

-   `Day` -- Day of the month
-   `Hour` -- Hour of the day
-   `Weekday` -- Day of the week represented numerically

## 🛠️ Technologies Used

-   **Python**
-   **Pandas** -- Data loading, transformation, and exploration
-   **Matplotlib** -- Data visualization
-   **Jupyter Notebook** -- Interactive analysis environment

## 🔍 Exploratory Data Analysis

### 1. Dataset Exploration

The notebook examines the dataset using:

``` python
uber_df.head()
uber_df.tail()
uber_df.shape
uber_df.info()
```

These operations help understand the records, dataset dimensions, and
column data types.

### 2. Date/Time Feature Engineering

The `Date/Time` column is converted from string format to Pandas
datetime format.

The notebook then extracts:

``` python
uber_df["Day"]
uber_df["Hour"]
uber_df["Weekday"]
```

This makes it possible to analyze ride demand at different time
intervals.

## 📊 Visualizations

The project creates visualizations for:

### 🚗 Trips by Day

A histogram is used to examine the density of Uber trips across days of
the month.

**Observation:** The analysis indicates that ride demand is generally
higher during working days compared with weekends.

### 📅 Trips by Weekday

A histogram shows the distribution of rides across the days of the week.

**Observation:** Monday is identified as the busiest weekday, while
Saturday has the lowest number of rides in the notebook's analysis.

### ⏰ Trips by Hour

A histogram is used to understand how trip demand changes throughout the
day.

**Observation:** The notebook identifies **6 PM** as the hour with the
highest number of rides.

### 📍 Trips by Location

A scatter plot using latitude and longitude is created to visualize the
geographical distribution of trips.

**Observation:** The notebook identifies areas near **Manhattan and
Newburgh** as having higher ride density, while the lowest density is
observed near **New Jersey**.

## 💡 Key Insights

Based on the analysis performed in the notebook:

-   Uber trip demand varies significantly throughout the month.
-   Weekday and weekend ride patterns are different.
-   **Monday** is identified as the busiest day of the week.
-   **Saturday** has the lowest number of rides among the weekdays
    analyzed.
-   Ride demand changes considerably throughout the day.
-   **6 PM** is identified as the peak hour in the analysis.
-   Geographic visualization shows concentrated ride activity around
    specific locations.

## 📁 Project Structure

``` text
Uber-Trips-Analysis/
│
├── Uber Trips Analysis.ipynb
├── uber-raw-data-sep14.csv
└── README.md
```

## ▶️ How to Run

### 1. Clone the repository

``` bash
git clone <your-repository-url>
cd Uber-Trips-Analysis
```

### 2. Install dependencies

``` bash
pip install pandas matplotlib jupyter
```

### 3. Make sure the dataset is available

Place:

``` text
uber-raw-data-sep14.csv
```

in the same directory as the notebook.

### 4. Launch Jupyter Notebook

``` bash
jupyter notebook
```

Open:

``` text
Uber Trips Analysis.ipynb
```

and run the cells sequentially.

## 📌 Project Objective

This project demonstrates fundamental **Exploratory Data Analysis,
feature engineering, and data visualization** skills using a real-world
Uber trips dataset.

It can be used as a beginner-friendly data analytics portfolio project
to demonstrate practical experience with **Python, Pandas, Matplotlib,
and EDA**.

## 👤 Author

**Aman**

If you find this project useful, feel free to ⭐ the repository.
