# **Bike Sharing Demand Prediction**

This project focuses on predicting bike-sharing demands using historical data. The main objective is to develop a machine learning model to help providers optimize bike availability and improve user satisfaction by forecasting hourly demands.

---

## **Part 1: Data Analysis and Preprocessing**

### **Dataset**

The dataset, sourced from Kaggle, contains historical data on bike rentals and includes features such as:
- **Datetime**: Hourly timestamps.
- **Weather Conditions**: Temperature, humidity, and windspeed.
- **Seasonal Information**: Season, holiday, and working day indicators.
- **Demand**: Number of total bike rentals.

---

### **Libraries Used**

The following Python libraries were used for analysis and model development:
- **pandas**  
- **numpy**  
- **matplotlib**  
- **scikit-learn**

---

### **Exploratory Data Analysis (EDA)**

Key insights from the data exploration include:
- A strong correlation between temperature and bike demand.
- Demand spikes during holidays and weekends, particularly in warmer weather.
- Certain weather conditions (e.g., heavy rain) reduce demand significantly.

---

### **Data Preprocessing**

1. **Feature Engineering**:  
   - Extracted time-based features (hour, day, month) from the `datetime` column.  
   - Created interaction terms to capture relationships between weather conditions and time-related variables.

2. **Encoding**:  
   - Transformed categorical variables (season, weather) using one-hot encoding.

3. **Scaling**:  
   - Normalized numerical variables (e.g., temperature, humidity) to ensure consistency.

---

## **Part 2: Model Development**

### **Model Selection**

After experimenting with several algorithms, **Random Forest Regressor** was chosen due to its superior performance in capturing nonlinear relationships in the data.

---

### **Model Evaluation**

The model achieved the following performance metrics:
- **Mean Absolute Error (MAE)**: 0.54  
- **Mean Squared Error (MSE)**: 0.49  
- **R² Score**: 0.76  

Despite overfitting challenges, careful tuning of hyperparameters and feature engineering improved generalization.

---

### **Visualization**

Key visualizations include:
1. **Correlation Matrix**: Highlighting relationships among features.  
2. **Residual Plot**: Revealing areas where the model struggles to predict demand accurately.  
3. **Actual vs. Predicted Values**: Demonstrating the model's overall predictive accuracy.

---

## **Usage**

To replicate this project locally, follow these steps:

1. **Install Required Libraries**:  
   Install the necessary dependencies:  
   ```bash```
   ```pip install pandas numpy scikit-learn matplotlib```

2. **Run The Notebook**:  
   Open and execute the provided Jupyter Notebook to reproduce results.

## **Contributing**

Contributions are welcome! Suggestions for improving the model or adding additional features can be submitted via:
   *Issues.*
   *Pull issues.*

## **Author**

**Ahmed AlSakka**

## **Acknowledgements**

Special thanks to Kaggle for providing the dataset and to the open-source contributors of Python libraries used in this project.