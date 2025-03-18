# **Walmart Stock Prices Prediction Using Statistical Models**  

## **Project Overview**  
This project analyzes and forecasts Walmart stock prices using statistical time-series models: **SARIMA** and **Holt-Winters Exponential Smoothing**. The research compares these models to determine the most effective forecasting method for predicting stock price trends from **2024 to 2028**. The dataset consists of over **20 years of historical stock prices** sourced from **Yahoo Finance**.  

## **Dataset**  
- **Source**: Yahoo Finance  
- **Period Covered**: January 2000 – October 2024  
- **Key Features**:  
  - Date  
  - Open, High, Low, Close Prices  
  - Adjusted Close Price  
  - Trading Volume  

## **Methodology**  
- **Data Preprocessing**:  
  - Handling missing values  
  - Converting date format  
  - Resampling to monthly data  
- **Models Used**:  
  - **SARIMA** (Seasonal AutoRegressive Integrated Moving Average)  
  - **Holt-Winters Exponential Smoothing**  
- **Performance Metrics**:  
  - **Mean Absolute Error (MAE)**  
  - **Root Mean Squared Error (RMSE)**  
  - **Akaike Information Criterion (AIC) for SARIMA**  

## **Results & Findings**  
- **SARIMA Model**:  
  - Best suited for seasonal stock price forecasting  
  - **Lowest MAE (2.53) and RMSE (3.15)**  
  - Captures long-term trends and seasonal patterns effectively  
- **Holt-Winters Model**:  
  - Simpler and computationally efficient  
  - Struggles with long-term forecasting accuracy  
  - **Higher MAE (8.07) and RMSE (8.84)**  

## **Conclusion**  
- **SARIMA is the most effective** model for forecasting Walmart stock prices due to its ability to handle **seasonality and trends**.  
- **Holt-Winters is a simpler alternative** but has **higher uncertainty** in long-term predictions.  
- Future work could integrate **macroeconomic indicators** and **machine learning models** to improve forecasting accuracy.  

## **Setup & Requirements**  
### **Prerequisites**  
- **Python 3.x**  
- **Google Colab / Jupyter Notebook**  

### **Required Libraries**  
Install dependencies using:  
```bash
pip install pandas numpy matplotlib statsmodels pmdarima seaborn
```

### **Running the Code**  
1. Open the Jupyter Notebook (.ipynb) in **Google Colab or Jupyter Notebook**.  
2. Upload the **Yahoo Finance dataset (CSV file)**.  
3. Run all cells to preprocess data, train models, and generate forecasts.  

## **File Structure**  
```
📁 walmart_stock_prediction/
├── 📄 README.md        # Project documentation  
├── 📄 *.ipynb          # Jupyter Notebook for analysis  
├── 📄 dataset.csv      # Walmart stock data  
└── 📄 requirements.txt # Required dependencies  
```

## **License**  
This project is licensed under the **MIT License**.

## **Acknowledgments**  
- **University of Hertfordshire** for guidance and academic support.  
- **Yahoo Finance** for providing open-access financial data.  