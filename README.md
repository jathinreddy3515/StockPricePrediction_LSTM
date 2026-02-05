# 📈 Stock Market Price Prediction Using LSTM

## 📌 Project Overview
This project predicts **future stock prices** using a **Long Short-Term Memory (LSTM)** neural network.  
LSTM is a type of **Recurrent Neural Network (RNN)** that is well-suited for **time-series forecasting**, especially financial data where past trends influence future values.

The model is trained on **historical stock price data** and learns patterns to forecast future closing prices.

---

## 🎯 Objectives
- Understand time-series data preprocessing
- Apply LSTM for stock price prediction
- Visualize actual vs predicted stock prices
- Build an end-to-end deep learning workflow

---

## 🧠 Whiteboard Explanation (Simple Terms)

Imagine stock prices like a **story over time**:
- Yesterday’s price affects today
- Today affects tomorrow

Traditional ML models forget old data.  
👉 **LSTM remembers important past information** using memory cells.

### How LSTM Works (High Level)
1. Takes past stock prices as input
2. Decides what to **remember** and **forget**
3. Learns long-term trends
4. Predicts the next stock price

---

## 🗂️ Project Structure
📦 stock-market-lstm
┣ 📜 stock_prediction_market_using_lstm.ipynb
┣ 📜 README.md
┗ 📂 dataset


---

## 📊 Dataset Details
- Historical stock price data
- Columns typically used:
  - `Date`
  - `Open`
  - `High`
  - `Low`
  - `Close`
  - `Volume`

> The **Close price** is used for prediction because it reflects the final market sentiment of the day.

---

## ⚙️ Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## 🔄 Workflow Steps (End-to-End)

### 1️⃣ Import Libraries
Load all required Python libraries for data processing, visualization, and modeling.

---

### 2️⃣ Load Dataset
Read historical stock data into a Pandas DataFrame.

---

### 3️⃣ Data Preprocessing
- Handle missing values
- Select `Close` price
- Normalize data using **MinMaxScaler**
- Create sequences (time steps)

**Why scaling?**  
LSTM works better when values are between 0 and 1.

---

### 4️⃣ Train-Test Split
- Training set: Learn patterns
- Testing set: Evaluate performance

Time-series data is **not shuffled** to preserve order.

---

### 5️⃣ Build LSTM Model
Model architecture:
- LSTM layer(s)
- Dropout (to avoid overfitting)
- Dense output layer

---

### 6️⃣ Model Training
- Loss function: Mean Squared Error (MSE)
- Optimizer: Adam
- Epochs & batch size tuned for performance

---

### 7️⃣ Predictions
- Predict stock prices on test data
- Convert scaled values back to original price range

---

### 8️⃣ Visualization
Plot:
- Actual stock prices
- Predicted stock prices

This helps visually evaluate model accuracy.

---

## 📈 Results
- The model successfully captures stock price trends
- Predictions closely follow actual prices
- Minor deviations due to market volatility

---

## 🧪 Model Evaluation
- **Evaluation Metric:** Mean Squared Error (MSE)
- **Interpretation:**  
  Lower MSE indicates better prediction accuracy and smaller error between actual and predicted values.

---

## 🚀 Future Improvements
- Use multiple input features (Open, High, Low, Volume)
- Implement **Bidirectional LSTM**
- Add technical indicators such as **RSI** and **MACD**
- Perform hyperparameter tuning for better model performance
- Integrate real-time stock market data using APIs

---

## 📌 Key Learnings
- Time-series data requires **sequential modeling**
- LSTM effectively captures **long-term dependencies**
- Data preprocessing and scaling are critical for deep learning models

---

## 👤 Author
**Jathin**


