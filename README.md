# 📈 Financial Stock Price Analysis Using Python
This project analyzes stock market data using Python to explore **price trends**, **returns**, and **volatility** of different companies over time.  
It applies basic **time series analysis** and **visualization** techniques to extract insights and understand stock behavior.

## ⚙️ Features & Objectives
- Analyze daily and monthly stock returns  
- Compare price trends between companies  
- Calculate and visualize moving averages  
- Examine volatility over time  
- Study correlation between multiple stocks  

## 🧩 Steps Performed
### 1. Data Collection
- Imported historical stock data (CSV format)
- Cleaned and structured it for time series analysis

### 2. Data Cleaning
- Handled missing values (if any)
- Converted date columns to datetime format
- Set the "Date" column as the index

### 3. Exploratory Data Analysis (EDA)
#### A. Price Trends
- Line plots showing the **closing price** of each stock over time
- Compared **growth and trends** between companies

#### B. Daily & Monthly Returns
- Calculated **daily returns**:  
  ```
  Daily Return = (Pt - Pt-1) / Pt-1
  ```
- Computed **monthly returns** using:
  ```python
  df.resample('M').mean()
  ```
- Visualized return distributions using histograms to observe volatility

#### C. Moving Averages & Volatility
- Computed 50-day and 200-day moving averages for long/short-term trends
- Used rolling standard deviation to measure volatility
- Plotted them together with stock prices

#### D. Correlation Between Stocks
- Calculated correlation matrix between daily returns
- Visualized relationships using a Seaborn heatmap — shows how closely different stocks move together

## 📊 Visualizations
- **Line Plot** → Stock price trends over time
- **Histogram** → Distribution of returns
- **Boxplot** → Compare volatility between stocks
- **Heatmap** → Correlation between stock returns

## 🧰 Technologies Used
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical computations
- **Matplotlib / Seaborn** – Data visualization

## 💡 Insights Gained
- Stocks show clear trends and seasonal patterns
- Moving averages smoothen short-term fluctuations
- High volatility periods can be easily identified
- Strong correlations indicate market-linked movement between companies
