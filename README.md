# Datascientists Job Insights Documentation

![GitHub License](https://img.shields.io/github/license/Sambonic/datascientists-job-insights)
![GitHub Issues](https://img.shields.io/github/issues/Sambonic/datascientists-job-insights)
![GitHub Top Language](https://img.shields.io/github/languages/top/Sambonic/datascientists-job-insights)
![Project Status](https://img.shields.io/badge/status-active-brightgreen)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)

This project analyzes data scientist salary data to identify correlations between salary, company attributes, and skills.

#### Last Updated: January 18th, 2025

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Features](#features)

<a name="installation"></a>
## Installation

Make sure you have [python](https://www.python.org/downloads/) downloaded if you haven't already.
Follow these steps to set up the environment and run the application:

1. Clone the Repository:
   
```bash
git clone https://github.com/Sambonic/datascientists-job-insights
```

```bash
cd datascientists-job-insights
```

2. Create a Python Virtual Environment:
```bash
python -m venv env
```

3. Activate the Virtual Environment:
- On Windows:
  ```
  env\Scripts\activate
  ```

- On macOS and Linux:
  ```
  source env/bin/activate
  ```
4. Ensure Pip is Up-to-Date:
  ```
  python.exe -m pip install --upgrade pip
  ```
5. Install Dependencies:

   ```bash
   pip install -r requirements.txt
   ```

6. Import Datascientists Job Insights as shown below.


<a name="usage"></a>
## Usage
1.  **Run the Jupyter Notebook:** Execute the `main-repo/src/data_scientist_salary_analysis.ipynb` notebook using a Jupyter Notebook environment.

2.  **Data Exploration:** The notebook reads and preprocesses two datasets (`data_cleaned_2021.csv` and `glassdoor_scraped.csv`), merging them for comprehensive analysis.  Observe the output of `df1.head()` and `df2.head()` to examine the initial data.

3.  **Data Visualization:** The code generates various visualizations, including histograms, bar plots, box plots, pie charts, bar charts, heatmaps, scatter plots, and KDE plots to represent data distributions and relationships between variables. Examine the generated plots to understand data insights.  These plots visualize salary distributions, company ownership types, sector distributions, industry-wise average salaries and ratings, job locations, skill distributions, and correlations between variables like age, required skills, and average salary.

4.  **Statistical Analysis:** The notebook performs statistical tests, such as correlation analysis and Chi-squared tests to determine the statistical significance of relationships between variables (e.g., the relationship between company rating and average salary, and the relationship between industry and salary range). Interpret the p-values to determine statistical significance.


<a name="features"></a>
## Features
- **Data Cleaning and Preprocessing:** Cleans and preprocesses two datasets (`data_cleaned_2021.csv` and `glassdoor_scraped.csv`), handling missing values, inconsistencies in salary and revenue formats, and standardizing data types.  Includes functions for data extraction and transformation.

- **Feature Engineering:** Creates new features such as `Lower Salary`, `Upper Salary`, `Avg Salary(K)`, `Lower Revenue`, `Upper Revenue`, `Lower Size`, `Upper Size`, `company_age`, and binarizes seniority.

- **Data Integration:** Merges the cleaned datasets based on common columns.

- **Exploratory Data Analysis (EDA):** Performs EDA using histograms, bar plots, box plots, and pie charts to visualize data distributions and relationships between variables (e.g., salary vs. type of ownership, industry analysis).

- **Salary Analysis:** Analyzes average salaries across different industries and sectors, identifying top-paying industries and their average ratings.  Visualizes findings with bar charts and scatter plots.

- **Geographic Analysis:** Identifies top locations for data science jobs and visualizes the average salaries in these locations using heatmaps and bar charts.

- **Skill Analysis:**  Analyzes the frequency of skills mentioned in job descriptions and correlates skill sets with age and average salary using regression plots, bar plots, box plots and heatmaps.

- **Company Analysis:** Analyzes the distribution of company types (public vs. private) across different states and correlates company type with average rating using line plots and scatter plots.

- **Revenue and Size Analysis:** Analyzes the distribution of company revenue and size and their correlation with salary using kernel density plots and heatmaps.

- **Statistical Testing:** Performs hypothesis testing (t-test and chi-squared test) to determine statistical significance of relationships between variables (e.g., rating and average salary, industry and average salary).


