# 🧪 Hate Speech Detection using TF-IDF and Logistic Regression

This project builds a simple but effective machine learning pipeline for Turkish hate speech detection using TF-IDF vectorization and a logistic regression classifier.

The project also applies a different approach to the first project which focuses on the same topic. You can visit here: [1eclerc's Repository | Hate Speech Detection on Turkish Tweets](https://github.com/1eclerc/Hate-Speech-Detection-on-Turkish-Tweets)

---

## 📌 Project Overview

- **Language**: Turkish
- **Goal**: Binary classification (hate speech vs non-hate speech)
- **Algorithm**: TF-IDF + Logistic Regression
- **Evaluation**: 5-Fold Cross-Validation with F1 Score

---

## 🗃️ Dataset

The dataset is read from an Excel file named `dataset_lemmatized.xlsx`.

| Column   | Description               |
|----------|---------------------------|
| `TEXT`   | Preprocessed Turkish tweet |
| `labels` | 0 (non-hate) or 1 (hate)   |

---

## 🔍 Model Details

- **Text Vectorization**: TF-IDF (`max_features=5000`)
- **Classifier**: Logistic Regression (`max_iter=1000`)
- **Evaluation**: `cross_val_score` with F1 scoring

### Sample Output:
```python
TF-IDF F1 Score Mean: 0.84
TF-IDF F1 Score Std Dev: 0.02
```

> Results may vary depending on the dataset quality and balance.

---

## 🚀 How to Run

### 1. Install required packages:
```bash
pip install pandas numpy scikit-learn gensim xgboost lightgbm openpyxl matplotlib seaborn
```

### 2. Prepare your data:
Place your dataset as `dataset_lemmatized.xlsx` with `TEXT` and `labels` columns.

### 3. Run the notebook:
Use Google Colab or Jupyter Notebook to execute the pipeline.

---

## 🛠 Tech Stack

- Python 🐍
- Scikit-learn
- Pandas
- NumPy
- TF-IDF Vectorizer
- Logistic Regression

---

## 📄 License

MIT License
