# 📈 NIFTY 50 Stock Price Prediction (ML & Deep Learning)

This project focuses on predicting **NIFTY 50 index prices** using a combination of **traditional Machine Learning** and **Deep Learning** models.  
The objective is to analyze how different models perform on **time-series stock data** across multiple historical window sizes.

## 🚀 Project Highlights

- End-to-end **time-series forecasting pipeline**
- Comparison between **ML vs DL models**
- Multiple **historical time windows (30–250 days)**
- Evaluation using **MAE** and **RMSE**
- Visualization of **model performance trends**
- Scalable and reusable training framework

---

## 📊 Features Used

- `Open`
- `Close`
- `High`
- `Low`

Each feature is converted into supervised learning format using a **sliding window approach**.

---

## 🛠️ Tech Stack

- **Python**
- **NumPy / Pandas**
- **Scikit-learn**
- **TensorFlow / Keras**
- **XGBoost**
- **LightGBM**
- **Matplotlib**
- **Joblib**

---

## 🧠 Models Implemented

### 🔹 Machine Learning Models
- Linear Regression
- Ridge Regression
- Lasso Regression
- K-Nearest Neighbors (KNN)
- Support Vector Regressor (SVR)
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- LightGBM Regressor

### 🔹 Deep Learning Models
- Simple RNN
- LSTM
- GRU
- Bidirectional LSTM

---

## 🧩 Data Preparation

- Sliding window technique used to create sequences
- Input windows range from **30 to 250 days**
- Target value is the **next day price**
- Data split into **90% training** and **10% testing**

---

## 🏋️ Model Training

- ML models trained using flattened time-series inputs
- DL models trained using 3D tensors `(samples, timesteps, features)`
- Optimizer: **Adam**
- Loss Function: **Mean Squared Error**
- DL models trained for multiple epochs
- Batch size optimized for faster convergence

---

## 📈 Evaluation Metrics

Models are evaluated using:

- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

Both **training** and **testing** errors are tracked to analyze generalization.

---

## 📊 Visualization & Analysis

- Train vs Test MAE comparison
- Model performance ranking
- Time-window frequency analysis among top models
- Model-type dominance in best performing results
- Trend analysis across different window sizes

---

## 🏆 Key Observations

- Deep Learning models outperform traditional ML models for longer sequences
- LSTM and Bidirectional LSTM show consistent improvement with larger windows
- Medium to long time windows (60–120 days) provide better predictive stability
- Tree-based models perform competitively on shorter windows

---

## 💾 Model Persistence

- All trained models and metrics are stored using `joblib`
- Enables reuse without retraining
- Results exported to CSV for easy analysis

---

## 📂 Project Structure

