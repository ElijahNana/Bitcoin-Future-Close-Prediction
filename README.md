 Bitcoin Future Close Prediction Using Machine Learning

This project focuses on analysing and modelling historical Bitcoin price data using machine learning techniques. It covers data cleaning, exploratory analysis, feature selection, and the implementation of predictive models to estimate future close prices. The project is intended to demonstrate practical data science skills applied to a real-world time series dataset.

Dataset

Source: [Kaggle – Bitcoin Historical Data](https://www.kaggle.com/datasets/mczielinski/bitcoin-historical-data)
Description: Daily historical Bitcoin data from 2012 to 2021, including Open, High, Low, Close prices, and Volume.

Columns:

  Date: Date of record
  Open: Opening price
  High: Highest price of the day
  Low: Lowest price of the day
  Close: Closing price
  Volume: Daily trading volume

 Project Highlights

Data Preprocessing: Converted date formats, handled missing values, and cleaned the dataset.
Exploratory Data Analysis: Visualised price trends, volatility, and price ranges across the dataset.
Outlier Analysis: Investigated anomalies in Volume data and explained why extreme values were retained.
Feature Engineering: Derived new variables and selected meaningful features using correlation and model-based importance techniques.

Machine Learning Models:

  - Decision Tree Regressor (for determining feature importance)
  - Random Forest Regressor
  - Linear Regression
  - K-Nearest Neighbours (KNN) Regressor
Evaluation: Models were evaluated using RMSE and visual comparison of predicted versus actual values.

Tools & Libraries

- Jupyter Notebook
- Python
- Pandas
- NumPy
- Matplotlib & Seaborn
- Scikit-learn

 Getting Started

1. Download or clone the repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Run the notebook:
   Open the `.ipynb` file in Jupyter Notebook or VSCode and follow the steps within.

 Results

After evaluating the models, Random Forest did not yield the best performance despite its complexity mainly due to lack of hyperparameter tuning. Simpler models like Linear Regression performed comparably or better depending on the metric used (i.e. RMSE). This highlights the importance of evaluating multiple approaches rather than relying solely on model complexity.


 Additional Notes

- A time-series train-test split was used to preserve the chronological order of data.
- Outliers in Volume were retained as they represent valid market activity rather than noise.
