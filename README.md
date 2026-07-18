# 🏠 House Price Prediction

> A beginner-friendly machine learning project that predicts house prices using Python and scikit-learn.

---

## 📌 What Does This Project Do?

This project teaches you how to **predict house prices** using machine learning. You'll learn how to:

- Look at and understand a dataset (EDA)
- Clean and prepare data for a model
- Train **3 different ML models** and compare them
- Figure out which features matter most for predicting price

No prior ML experience needed — every step is clearly commented!

---

## 🧠 Machine Learning Models Used

| Model | What It Does |
|---|---|
| **Linear Regression** | Draws a straight line through the data to make predictions. Simple and fast. |
| **Decision Tree** | Asks a series of yes/no questions to arrive at a prediction. Easy to visualize. |
| **Random Forest** | Combines hundreds of decision trees and averages their predictions. Usually the most accurate. |

---

## 📊 The Dataset

No need to download anything — the dataset is **generated inside the notebook** itself!

It contains **500 fake-but-realistic houses** with these features:

| Feature | What It Means |
|---|---|
| `area` | Size of the house in square feet |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `stories` | Number of floors |
| `parking` | Number of parking spaces |
| `mainroad` | Is the house on a main road? (yes/no) |
| `basement` | Does it have a basement? (yes/no) |
| `location` | Urban, suburban, or rural? |
| `price` | 🎯 This is what we're trying to predict! |

---

## 🔢 How Are Prices Calculated?

Prices are built using a realistic formula so the models have something meaningful to learn:

```
price = (area × 150 + bedrooms × 25,000 + bathrooms × 15,000
         + stories × 20,000 + parking × 10,000)
        × location_factor × mainroad_factor × basement_factor
        + random noise
```

- 🏙️ Urban houses cost more than 🌳 rural ones
- Main road access and basements add a small price boost
- Random noise is added to make the data realistic

---

## 📁 Project Steps (Step-by-Step)

The notebook has **25 numbered steps**:

| Steps | What Happens |
|---|---|
| 1–2 | Import libraries and generate the dataset |
| 3–6 | Preview the data (first rows, shape, stats) |
| 7–8 | Check for missing values, duplicates, and plot distributions |
| 9–11 | Visualize correlations and relationships |
| 12 | Clean the data and encode text columns into numbers |
| 13 | Create a new feature: `rooms_per_story` |
| 14–15 | Select features and split into training/testing sets (80/20) |
| 16–18 | Train and evaluate Linear Regression |
| 19–21 | Train and evaluate Decision Tree |
| 22–24 | Train and evaluate Random Forest |
| 21 | Compare all 3 models side by side |
| 22–23 | See which features matter most (Feature Importance) |
| 24–25 | Automatically find the best model and explain the results |

---

## 📏 How Do We Measure Performance?

Three metrics are used to judge each model:

| Metric | What It Tells You | Better When... |
|---|---|---|
| **MAE** (Mean Absolute Error) | Average dollar amount the model is off by | Lower ✅ |
| **RMSE** (Root Mean Squared Error) | Similar to MAE but penalises big mistakes more | Lower ✅ |
| **R²** (R-squared) | How much of the price variation the model explains (0 to 1) | Closer to 1 ✅ |

---

## ⚙️ Requirements

Make sure you have Python 3.x installed, then install the required libraries:

```bash
pip install numpy pandas matplotlib scikit-learn
```

---

## ▶️ How to Run

1. Open a terminal and navigate to the project folder
2. Launch Jupyter:

```bash
jupyter notebook house_price_prediction_1784393001786.ipynb
```

3. Run all cells from top to bottom using **Kernel → Restart & Run All**

That's it! No dataset file needed — everything is generated for you. 🎉

---

## 💡 Key Concepts You'll Learn

- **EDA (Exploratory Data Analysis)** — understanding your data before modelling
- **Label Encoding** — converting text categories (like "yes"/"no") into numbers
- **Feature Engineering** — creating new useful columns from existing ones
- **Train-Test Split** — keeping some data hidden to test how well the model really works
- **Feature Importance** — finding out which inputs have the biggest effect on predictions

---

## 🙋 Need Help?

If something doesn't work:
- Make sure all libraries are installed (`pip install ...`)
- Make sure you're running cells **in order** from top to bottom
- Re-run the kernel if you get a "variable not defined" error (**Kernel → Restart & Run All**)
