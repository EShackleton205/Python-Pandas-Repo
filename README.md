# Python-Pandas-Repo
A place to put all of my pandas projects.

# Python Data Analysis Project

## Overview

This project was completed as part of a **Data Technician Bootcamp** and focuses on using **Python** and **pandas** for data analysis, data cleaning, and visualization. The project involved exploring retail and sales datasets to identify trends, improve data quality, and generate insights through statistical analysis and visual reporting.

## Key Skills Demonstrated

### Data Loading and Exploration
- Importing datasets into Python using **pandas**
- Exploring dataset structure using:
  - `head()`
  - `info()`
  - `describe()`
  - `shape`
  - `columns`
- Understanding data types and identifying data quality issues

### Data Filtering and Slicing
- Filtering records using conditional logic
- Selecting specific rows and columns with:
  - `.loc[]`
  - `.iloc[]`
- Creating focused subsets of data for targeted analysis
- Extracting data based on sales regions, product categories, dates, and performance metrics

### Data Cleaning and Preparation
- Handling missing values using:
  - `dropna()`
  - `fillna()`
- Removing duplicates and correcting inconsistencies
- Converting data types where required
- Preparing datasets for analysis and visualization

### Data Manipulation with Pandas
Used a variety of pandas methods to transform and analyse data:

- `groupby()`
- `sort_values()`
- `dropna()`
- `fillna()`
- `value_counts()`
- `reset_index()`
- `rename()`
- `merge()`
- `astype()`

These methods were used to organize, summarize, and transform retail and sales data into meaningful business information.

## Retail & Sales Data Analysis

The project applied data analysis techniques to answer business-focused questions such as:

- Which products generate the highest sales?
- Which regions contribute the most revenue?
- What trends can be identified over time?
- Which product categories perform best?
- How does customer purchasing behaviour vary across different segments?
- Are there any patterns in sales growth or decline?

Using pandas, large datasets were transformed into summary tables and key performance indicators that supported data-driven decision-making.

## Data Visualization

Visualizations were created using pandas plotting functionality and **Matplotlib** to communicate findings effectively.

### Visualizations Included

- Bar Charts
- Line Charts
- Pie Charts
- Histograms
- Trend Analysis Charts

These visualizations helped to:

- Compare product and regional performance
- Track sales trends over time
- Identify outliers and unusual patterns
- Present insights in an accessible and professional format

## Example Techniques Used

### Filtering Data

```python
high_sales = sales_data[sales_data["Sales"] > 1000]
```

### Using `.loc[]`

```python
sales_data.loc[sales_data["Region"] == "North"]
```

### Using `.iloc[]`

```python
sales_data.iloc[0:10, 0:5]
```

### Grouping and Aggregating Data

```python
sales_by_region = (
    sales_data
    .groupby("Region")["Sales"]
    .sum()
    .reset_index()
)
```

### Sorting Results

```python
sales_data.sort_values(by="Sales", ascending=False)
```

### Filling Missing Values

```python
sales_data["Sales"].fillna(0, inplace=True)
```

### Creating a Visualization

```python
import matplotlib.pyplot as plt

sales_by_region.plot(
    kind="bar",
    x="Region",
    y="Sales"
)

plt.title("Sales by Region")
plt.show()
```

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Google Colab

## Skills Applied

- Data Cleaning
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Summarization
- Problem Solving
- Data Quality Management
- Business Intelligence

## Learning Outcomes

Through this project, I developed practical experience in:

- Loading and analysing real-world datasets with pandas
- Filtering and slicing data using `.loc[]` and `.iloc[]`
- Cleaning and preparing data for analysis
- Using pandas functions to manipulate and summarize information
- Creating visualizations to communicate insights effectively
- Identifying trends and patterns within retail and sales datasets
- Supporting business decision-making through data analysis

## Project Outcome

This project demonstrates the use of Python as a powerful data analysis tool. By combining pandas data manipulation techniques with visualization libraries such as Matplotlib, I was able to explore, clean, analyse, and present retail and sales data in a meaningful way. The resulting analysis transformed raw datasets into actionable insights that support reporting, trend identification, and data-driven business decisions.
