# Tesla Stock Price Prediction using Facebook Prophet

This project uses the **Facebook Prophet**, an open-source tool from Facebook, to forecast **Tesla (TSLA) stock closing prices** based on past one year of historical data. The dataset is pulled directly from **Yahoo Finance** and analyzed using **Python** with interactive visualizations.

---

## 🔍 Overview

Stock price forecasting helps investors and analysts understand market trends and make informed decisions.

### Key Objectives:

- Fetch Tesla’s historical stock data using **Yahoo Finance**
- Perform **exploratory data analysis (EDA)** and visualize stock trends
- Build and train a **Prophet forecasting model**
- Generate a **30-day future price prediction**
- Compare **actual vs predicted prices**
- Export forecast results for evaluation and further use

---

## 📁 Project Files

1. **`Tesla Stock Price Data Evaluation - Sheet1.csv`** → Processed Tesla stock dataset in CSV format  
2. **`Tesla Stock Price Data Evaluation.xlsx`** → Dataset in Excel format for inspection  
3. **`Tesla_Stock_Price_Prediction_using_Facebook_Prophet.ipynb`** → Jupyter Notebook with full implementation  

---

## 📊 Key Steps

### 1. Data Collection  
- Source: Yahoo Finance (`yfinance` library)  
- Timeframe: Last **1 year** (250 trading days)  

### 2. Exploratory Data Analysis (EDA)  
- Descriptive statistics (`.info()`, `.describe()`)  
- Visualizations:
  - Closing Price Trends (line & area charts)
  - Trading Volume (area & bar charts)
  - Distribution of Closing Prices (boxplot)

### 3. Data Preparation  
- Prophet requires:  
  - **`ds`** → Date  
  - **`y`** → Target (Closing Price)  

### 4. Prophet Modeling  
- Fitted with default settings (weekly seasonality enabled, daily/yearly disabled)  
- Future dataframe created for **30 additional days**  
- Predictions include: `yhat` (forecast), `yhat_lower`, `yhat_upper`

### 5. Visualization  
- Closing Price & Volume trends (line, area, bar charts)  
- Boxplot of closing prices  
- Prophet forecast and components  
- Actual vs forecast overlay  
- Next 30 days forecast   

### 6. Results Export  
- Forecast saved as `forecast.csv`  
- Download enabled in Google Colab  

---

## 📈 Forecast Output

- 📅 Predicted next 30 days of Tesla stock closing prices  
- 🔼 Confidence intervals (`yhat_lower`, `yhat_upper`) show prediction uncertainty  
- 📊 Visuals compare **historical data vs forecasted trend**  

---

## 🛠️ Tools & Libraries

- Python 3.x
- Pandas
- Plotly
- Prophet (Facebook Prophet)
- Yahoo Finance (`yfinance`)
- Google Colab

---

## ⚙️ How to Run

1. Clone the repository:
```bash
git clone https://github.com/zihanmanbit/ML-Projects.git
cd "ML-Projects/Tesla Stock Price Prediction using Facebook Prophet"
```

2. Install dependencies:
```bash
pip install pandas plotly prophet yfinance
```

3. Open the notebook:
```bash
jupyter notebook Tesla_Stock_Price_Prediction_using_Facebook_Prophet.ipynb
```

---

## 🎓 References

- Coursera Project: [Tesla Stock Price Prediction using Facebook Prophet](https://www.coursera.org/projects/tesla-stock-price-prediction-facebook-prophet)
- Credentials: [https://www.coursera.org/account/accomplishments/verify/A2MGKQWTZX8C](https://www.coursera.org/account/accomplishments/verify/A2MGKQWTZX8C)

---
