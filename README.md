# Communicable Disease Analysis Across California Counties
This repository contains Python code for building and analyzing rate prediction models using previous data as well as user interactive database querying.
## Features
1. Reading data from a CSV file.
2. Data cleaning and data insertion.
3. Data transformation:
   - Rate predicting using the ARIMA model.
   - Rate predicting using a Linear Regression model.
   - Rate predicting using a baseline model.
4. Database for querying about top diseases, case counts, and more.
5. Web scraping for Wikipedia links for each disease.

## Requirements
The following Python libraries are used:
   * pandas
   * scipy.stats
   * sklearn.metrics
   * matplotlib.pyplot
   * numpy
   * pmdarima
   * sklearn.preprocessing
   * sklearn.linear_model
   * sklearn.model_selection
   * sqlite3
   * requests
   * bs4
     
## Getting Started
1. Clone the repository:
   ```bash
   git clone <repository-url>
3. Navigate to the project folder:
   ```bash
   cd Communicable-Disease-Analysis-Across-California-Counties

## Usage
1. Generate Cleaned CSV File: Clean the data for analysis and insert rows for Sex = 'Other'
2. Create Data Visualizations: Visualize trends in the data with the scatter plots produced.
3. Run Prediction Models and Evaluate: 
   * Predict rates with the ARIMA model with previous data.
   * Show poor prediction with Linear Regression model.
   * Show baseline predictions with baseline model.
   * Evaluate models with mean squared/absolute error and/or r2 score.
4. Database Querying: Receive responses to common questions regarding the data.
5. User Inquiry: Input disease, county, and sex of choice to receive details about the case counts until 2022.
6. Explore Further Details about the Disease: Web scrape for the disease's Wikipedia page.

## Key Functions
`clopper_pearson_exact_method(cases, pop, alpha = 0.05)`: Calculates the lower and upper bound of 95% confidence interval for the incidence rate of the disease, given the case count and population of the county.  
`search_wiki(disease)`: Returns the link for the Wikipedia page about the disease including its causes, signs and symptoms, treatment options, and more.

## Video Demo
Click [here](https://drive.google.com/file/d/1qQ19F9aj8TB_0dy9YpAQfrTEzMS5oNf-/view?usp=sharing) to watch a demonstration video of the project.





