# 📈 Predicting Stock Price Direction using Support Vector Machines

## 🎯 Objective
Build a machine learning model to predict whether a stock’s price will **rise or fall the next day** using historical price data.

## 📊 Dataset
- Historical stock data (RELIANCE.csv) including Open, High, Low, Close.

## 🔑 Key Steps
1. **Data Preprocessing**  
   - Converted `Date` column to index  
   - Dropped unused columns  

2. **Feature Engineering**  
   - Created predictor variables: `Open–Close` and `High–Low` differences

3. **Target Variable**  
   - Next-day price movement  
   - `1` → Price goes up  
   - `0` → Price goes down  

4. **Train/Test Split**  
   - Sequential 80/20 split (no shuffling, to preserve temporal order) 

5. **Model Training**  
   - Implemented Support Vector Classifier (SVC)  

6. **Kernel Experiments**  
   - Linear, Polynomial, RBF, Sigmoid  

7. **Evaluation**  
   - Measured accuracy on training & testing sets  
   - Compared cumulative returns of SVM strategy vs. original stock returns  

## 🛠 Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- scikit-learn  

## ✅ Outcome
Developed an **end-to-end stock price direction prediction pipeline** and visualized how an **SVM-based strategy** compares with simply holding the stock.
