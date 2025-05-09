# 📈 Machine Learning Pipeline for Stock Prediction  
**Predicting Next-Day Stock Prices Using 10-K, 10-Q, and 8-K Filings**

---

## 🧠 Overview

This project demonstrates a comprehensive **Machine Learning (ML) pipeline** to predict **next-day stock prices** using **recently published SEC filings (10-K, 10-Q, and 8-K)**. The work was conducted as part of my **Master Thesis**, showcasing end-to-end data processing, model development, evaluation, and a trading simulation.

---

## 🏗️ Pipeline Architecture

### 🔬 Data Preprocessing

- Merging and cleaning financial text data (not included, done in another part)
- **Handling missing/corrupted values**
- **Data normalization** before training and **denormalization** for simulation
- Exploratory analysis of:
  - Training/test/validation splits
  - Distribution of 8-K vs. 10-K/10-Q filings
  - Label statistics and dataset health (e.g., NaNs)

### 📦 Dataset & Dataloader

- Custom `Dataset` using masked input arrays
- **Train/Test/Validation split**
- **Tensor shape adjustments** for compatibility
- Efficient loading using PyTorch's `DataLoader`

### 🤖 Model

- Implemented in **PyTorch**
- Simple **LSTM** model for time-series analysis
- Support for hyperparameter tuning and configuration

### 🔁 Training & Testing

- Training and evaluation loops with:
  - Loss tracking
  - Metric logging
- Explanation and impact of **key hyperparameters**

---

## 📊 Evaluation Metrics

### 📉 Regression Metrics
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-Squared (R²)

### 🧮 Classification Metrics
- Accuracy
- Precision / Recall / F1-Score
- Confusion Matrix

### 📊 Data Exploration
- Sample counts (train/test/val)
- Label count & distribution
- Change in values from today to next-day
- Comparison: 8-K vs. 10-K/Q filings
- NaN statistics and label prediction counts

---

## 📈 Visualizations

- 📚 **Learning Curves**
- 🧠 **SHAP (SHapley Additive exPlanations)** analysis for model interpretability
- 🗂️ Dataset distribution and breakdown charts
- 📉 Prediction vs. Ground Truth plots
- 📊 Confusion matrices

---

## 💰 Trading Simulation

A **simple 'All In' strategy simulation**, comparing:
- ✅ Our model's predictions
- 🧍‍♂️ Buy and Hold
- 🎲 Random Walk
- 📈 Always Long
- 📉 Always Short

### 🔧 Features:
- Customizable **commission fees** (e.g., $5/side in showcased run)
- Visualization of **equity curves**
- Tabular summary of simulated performance

---

## 🛠️ Technologies Used

- Python
- PyTorch
- Pandas / NumPy
- Matplotlib
- SHAP
- Scikit-learn

---

## 📚 License

This project is part of academic research and open for educational use. Please cite appropriately.

---

## 🙋‍♂️ Author

**Leonard Müller**  
Master Thesis - Julius-Maximilians-Universität Würzburg  
Contact: leonardmueller.lm@gmail.com  

