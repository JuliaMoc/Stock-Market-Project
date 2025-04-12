# Stock Market Project

## Overview

This project focuses on the analysis of the top 5 tech companies. The Kaggle dataset contains stock market data, specifically from the US stock market. The dataset includes stock prices and volume data for various sectors (commodities, cryptocurrency, tech companies, and other successful US companies) from 2019 to 2023. 
The project incorporates data processing, exploratory data analysis (EDA), and machine learning for stock price prediction.

Note: This is a self-initiated learning project using open-source data for practice and portfolio development.

## Table of Contents

1. Project Overview
2. Data Sources
3. Technologies Used
4. Data Processing
5. Files
6. Data Visualization
7. Machine Learning
8. How to Run the Project
9. License

### 1. Project Overview

The main objective of this project was to process and analyze historical stock data, focusing on the top 5 tech companies (Apple, Google, Microsoft, Meta, and Nvidia). Key tasks included:
- **Data Cleansing & Transformation:** Handling missing values, formatting dates, and creating new features (e.g., "Previous day prices", "Price differences", "Volume differences", etc.).
- **Comparative Analysis:** Comparing the stock performance of the top 5 tech companies.
- **Data Visualization:** Using Tableau to create interactive visualizations showing the stock performance of the top 5 tech companies.
- **Machine Learning:** Building a regression model using RandomForestRegressor to predict Apple's stock price for the future.

### 2. Data Sources

The dataset used in this project was sourced from Kaggle and includes stock prices and volumes for a variety of US companies from 2019 to 2023. It covers several sectors, including commodities, cryptocurrencies, and tech companies.

### 3. Technologies Used

- **Python:** Main programming language
- **Libraries:** Pandas (data manipulation), NumPy (numerical computations), Matplotlib (visualizations), Scikit-learn (machine learning)
- **Tableau Public:** Interactive visualizations

### 4. Data Processing

The raw Kaggle dataset required several preprocessing steps:
- **Formatting Dates:** Ensured that all dates were properly formatted for analysis.
- **Feature Engineering:** Added columns for "Previous day prices" and "Previous day volumes”. Calculated "Price differences" and "Volume differences" between consecutive days. Computed percentage differences for price and volume changes.
- **Focus on Tech Companies:** While the dataset contained data for all sectors, I focused on the top 5 tech companies (Apple, Google, Microsoft, Meta, and Nvidia) for comparison.

### 5. Files

- **Stock_Market_Dataset**: Original dataset from Kaggle.
- **Stock_Market_Dataset_Merged.csv**: This is the main merged dataset containing data from 2019 to 2023 for all companies in the dataset.
- **Stock_Market_Dataset_Share.csv**: Contains data for the top 5 tech companies (Apple, Google, Microsoft, Meta, and Nvidia).
- **Stock_Market_Dataset_Share_End.csv**: Contains the yearly closing prices for the top 5 tech companies, used for further analysis and visualizations in Tableau.
- **Tableau Visualization**: Tech Stock Performance (Also available on Tableau Public: https://public.tableau.com/app/profile/julia.mochel/viz/TECHSTOCKPERFORMANCETop5/Top5Performance).
- **Stock_Market_Data_Exploratory & Apple_Stock_Price_Prediction**: Jupyter notebooks containing all data processing, analysis, visualization code and price prediction.

### 6. Data Visualization

I used **Tableau Public** to create an interactive visualization that allows users to explore the performance of the top 5 tech companies (Apple, Google, Microsoft, Meta, and Nvidia). The key features of the visualization include:
- **Filter and Comparison Options:** Users can filter by year and compare the percentage change in stock prices and volumes across companies.
- **Min/Max Markers:** Highlighted the minimum and maximum prices for each filtered year.
- **Charts:** Line charts showing the changes in stock prices and volumes over time for each company. A table showing the maximum, minimum, and average prices, as well as the percentage change in stock prices and volumes. Additionally, two line charts were created to show the stock performance of the top 5 tech companies from 2019 to 2023.

### 7. Machine Learning

For future price prediction, I created a regression model to predict the stock price of Apple. Here are the details:
- **Data Preprocessing:** Filtered the dataset to only include Apple's stock prices and volumes.
- **Model:** Used a RandomForestRegressor model from Scikit-learn to predict future stock prices.
- **Evaluation:** The initial model score was 0.998264. Hyperparameter tuning using RandomizedSearchCV was performed, improving the model's score to 0.998265.

### 8. How to Run the Project

To run this project on your local machine, make sure that **Python** and **pip** are installed.
1. Clone this repository:
   ```bash
   git clone https://github.com/JuliaMoc/Stock-Market-Project.git
   cd Stock_Market_Project

2. Install the required Python libraries: 
   ```bash
   pip install -r requirements.txt
   
3. Run the Jupyter notebook or Python scripts to reproduce the analysis:
   ```bash
   jupyter notebook Stock_Market_Data_Exploratory.ipynb
   
4. Or run the machine learning model:
    ```bash
    jupyter notebook Apple_Stock_Price_Prediction.ipynb

5. Explore the **cleaned CSV dataset** (Stock_Market_Dataset_Merched.csv) for further analysis or use it in Tableau for additional visualizations.

5. Explore the Tableau visualization by visiting the link (https://public.tableau.com/app/profile/julia.mochel/viz/TECHSTOCKPERFORMANCETop5/Top5Performance) on Tableau Public.

### 9. License

This project is licensed under the MIT License - see the LICENSE file for details.
