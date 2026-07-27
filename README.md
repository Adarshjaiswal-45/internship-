# 🚗 Car Price Prediction
 
Predicting used car prices from historical specification data using regression models.
 
## 📌 Objective
 
Develop a machine learning model that predicts car prices based on historical data, helping buyers judge if a price is fair and helping sellers price a car competitively.
 
## 📊 Dataset
 
**Automobile Dataset** (Kaggle: [toramky/automobile-dataset](https://www.kaggle.com/datasets/toramky/automobile-dataset)), based on the classic UCI Automobile dataset — 205 vehicles with 26 attributes including make, engine specs, dimensions, fuel economy, and price.
 
> This repo includes `automobile_synthetic.csv` — a synthetic dataset generated with the **exact same column schema** as the real Kaggle data, so the notebook runs out of the box even without downloading anything. To use the real data instead, see [Using the real dataset](#using-the-real-dataset) below.
 
## 🛠️ Tools & Libraries
 
- Python 3
- Pandas / NumPy
- Scikit-Learn
- Matplotlib / Seaborn
- Jupyter Notebook
## 🔍 Project Steps
 
1. **Data Cleaning & Preprocessing** — handle missing values (`?` markers), fix numeric data types, impute gaps (median for numeric, mode for categorical)
2. **Exploratory Data Analysis (EDA)** — price distribution, correlation heatmap, relationships between price and engine size / horsepower / curb weight, price by body style
3. **Feature Engineering** — one-hot encoding of categorical variables
4. **Model Training & Evaluation** — Linear Regression, Ridge, Lasso, and Random Forest, compared using R², MAE, and RMSE
5. **Results** — actual-vs-predicted visualization and feature importance ranking
## 📈 Results
 
The models are compared on a held-out test set:
 
| Model             | R²   | MAE | RMSE |
|-------------------|------|-----|------|
| Linear Regression | —    | —   | —    |
| Ridge Regression   | —    | —   | —    |
| Lasso Regression   | —    | —   | —    |
| Random Forest      | —    | —   | —    |
 
*(See the notebook output for actual scores — Engine size, horsepower, and curb weight are consistently the strongest predictors of price.)*
 
## 🚀 Getting Started
 
### 1. Clone the repo
```bash
git clone https://github.com/<your-username>/car-price-prediction.git
cd car-price-prediction
```
 
### 2. Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```
 
### 3. Run the notebook
```bash
jupyter notebook Car_Price_Prediction.ipynb
```
 
## 📁 Using the Real Dataset
 
1. Download `automobile.csv` from [Kaggle](https://www.kaggle.com/datasets/toramky/automobile-dataset).
2. Place it in the project's root folder.
3. Re-run all notebook cells — Step 1 auto-detects the real CSV and uses it instead of the bundled synthetic data. No code changes needed.
## 📂 Repository Structure
 
```
car-price-prediction/
├── Car_Price_Prediction.ipynb    # Main notebook: cleaning, EDA, modeling, evaluation
├── automobile_synthetic.csv      # Schema-matched sample dataset (fallback / demo data)
└── README.md
```
 
## ✅ Outcome
 
A regression pipeline that delivers reasonably accurate car price predictions from vehicle specifications, aiding both buyers and sellers in making informed pricing decisions.
 
## 📄 License
 
This project is open source and available under the [MIT License](LICENSE).
