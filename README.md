# Movie-Success-Prediction-
# 🎬 Movie Success Prediction and Sentiment Analysis

## 📌 Objective
This project aims to **predict movie success** (based on box office revenue or IMDb rating) using publicly available data, and to **analyze viewer sentiment** through review texts using NLP.

---

## 🛠 Tools & Technologies
- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- NLTK (VADER Sentiment Analyzer)
- Excel (for basic cleaning or tabular exploration)

---

## 📊 Features & Data Used
- **Movie Metadata**: Budget, revenue, genre, runtime, IMDb rating
- **User Reviews**: Used for sentiment analysis with VADER
- **Derived Feature**: Sentiment polarity score for each review

---
## 🔍 Sentiment Analysis (VADER)
- Used NLTK’s **VADER SentimentIntensityAnalyzer**.
- Classified sentiments as:
  - **Positive** (compound ≥ 0.05)
  - **Neutral** (-0.05 < compound < 0.05)
  - **Negative** (compound ≤ -0.05)

### ✅ Visualizations:
- Histogram of compound sentiment scores
- Pie chart of sentiment distribution
- Bar chart of average sentiment by genre

---
## 🤖 Predictive Model
- **Goal**: Predict `revenue` using regression models.
- **Features Used**: Budget, runtime, sentiment score, genre
- **Models Tried**:
  - Linear Regression
  - Random Forest Regressor

### 📈 Evaluation:
| Metric              | Value          |
|---------------------|----------------|
| R² Score            | ~0.78          |
| Mean Squared Error  | ~1.2e+08       |

### ✅ Visuals:
- Scatter plot of Actual vs Predicted revenue
- Feature importance bar chart (Random Forest)
