# Task 2: Unemployment Analysis with Python

## 📌 Project Overview

This project focuses on Exploratory Data Analysis (EDA) of unemployment data in India to identify regional and temporal trends, with particular emphasis on the impact of the COVID-19 pandemic on unemployment rates.

Using Python's data analysis and visualization libraries, the project explores unemployment rates across different states and regions, compares pre-COVID and post-COVID unemployment levels, and investigates relationships between unemployment, employment, and labour participation rates.

## 🎯 Objectives

- Analyze unemployment trends across Indian states and regions.
- Calculate and compare average unemployment rates by region.
- Examine month-wise and time-series unemployment trends.
- Identify the states with the highest average unemployment rates.
- Explore correlations between unemployment rate, employment rate, and labour participation rate.
- Compare unemployment rates before and after the COVID-19 pandemic.
- Present findings through clear and informative visualizations.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

## 📂 Project Structure

```text
OIBSIP/
└── DataScience-Task2-UnemplymentAnalysiswithPython/
    └── ├── README.md
        ├── Unemployment_Analysis_with_Python.ipynb
        └── data/
            └── unemployment.csv
```

*Note: Update the folder names and dataset filename to match your actual repository structure.*

## 📊 Dataset

The project uses an unemployment dataset containing information about Indian states and regions over time.

Expected variables may include:

- **Region:** State or region name.
- **Date:** Observation date.
- **Estimated Unemployment Rate (%):** Unemployment rate.
- **Estimated Employed:** Estimated number of employed people.
- **Estimated Labour Participation Rate (%):** Labour force participation rate.

The exact column names depend on the selected dataset.

## 🔍 Project Workflow

### 1. Data Loading and Inspection
- Load the dataset using Pandas.
- Inspect the number of rows and columns.
- Check data types and missing values.
- Convert date columns to the appropriate datetime format.
- Clean column names and handle missing or duplicate records.

### 2. Exploratory Data Analysis (EDA)
- Calculate average unemployment rates by region.
- Analyze monthly unemployment trends.
- Identify regional differences in unemployment.
- Examine the distribution of unemployment rates.

### 3. Data Visualization

The project includes the following visualizations:

- **Time-Series Line Chart:** Tracks unemployment rates over time for at least three major states or regions.
- **Bar Chart:** Highlights the top 10 states or regions with the highest average unemployment rates.
- **Correlation Heatmap:** Examines relationships between unemployment rate, employment, and labour participation rate.
- **Pre-COVID vs. Post-COVID Comparison:** Compares average unemployment rates across the two periods.
- **Regional Comparison Charts:** Visualize differences in unemployment rates between regions.

### 4. COVID-19 Impact Analysis

The dataset is divided into two periods using observation dates:

- **Pre-COVID:** Before the selected pandemic cutoff date.
- **Post-COVID:** On or after the selected pandemic cutoff date.

Mean unemployment rates are calculated for both periods. The difference is used to examine changes in unemployment across Indian states and regions.

The cutoff date and period definitions are documented in the notebook to ensure the comparison is transparent.

### 5. Insights and Observations

Markdown cells throughout the notebook explain the results of each analysis and visualization, including regional disparities, temporal patterns, and changes observed across the selected COVID-19 periods.

## ⚙️ Installation and Setup

### Prerequisites

Install Python 3.9 or later and Jupyter Notebook.

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run the Project

1. Clone or download the repository.
2. Place the dataset in the appropriate project directory.
3. Open a terminal in the project folder.
4. Launch Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `unemployment_analysis.ipynb`.
6. Update the dataset path if necessary.
7. Run all cells in sequence.

## 📈 Expected Outcomes

- Identification of regions with relatively high and low unemployment rates.
- Understanding of unemployment trends over time.
- Comparison of average unemployment rates before and after COVID-19.
- Insights into relationships between unemployment, employment, and labour force participation.
- A collection of visualizations supporting data-driven observations.

## ⚠️ Limitations

The analysis depends on the coverage, quality, and time range of the selected dataset. Changes between pre-COVID and post-COVID averages show associations over time and do not, by themselves, establish that COVID-19 caused those changes.

## 👨‍💻 Author

**Hazem Ebrahim**

Data Science Intern | Python | Data Analysis | Machine Learning

## 📜 Acknowledgment

This project is completed as part of **Task 2: Unemployment Analysis with Python** under the Oasis Infobyte Internship Program (OIBSIP).

---

*If you find this project useful, feel free to star the repository.*
