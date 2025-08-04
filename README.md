# Credit-card-detection# 💳 Credit Card Fraud Detection

This project uses **supervised machine learning** to detect fraudulent credit card transactions from an **imbalanced dataset** of over 284,000 records. The dataset is preprocessed, analyzed, and used to train a **Random Forest classifier**, with performance evaluated using relevant metrics like ROC-AUC and confusion matrix.

---

## 📂 Dataset

- **Source**: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Class Distribution**: Extremely imbalanced — only 492 fraud cases (~0.17%)
- **Features**: 30 features (V1–V28 are PCA-transformed), `Time`, `Amount`, and `Class` (target: 1 = fraud, 0 = legit)

---

## 🛠️ Tech Stack

- **Language**: Python 3
- **Libraries**:
  - `NumPy`, `Pandas` – data manipulation
  - `Seaborn`, `Matplotlib` – visualization
  - `Scikit-learn` – ML modeling and metrics

---

## 📊 Project Workflow

### 1. Data Exploration
- Visualized fraud vs. non-fraud class imbalance.
- Examined `Amount` and `Time` features.
- Checked feature correlations using heatmaps.

### 2. Preprocessing
- Scaled the `Amount` feature.
- Split dataset into training and testing sets (80/20).
- Optional: Could apply **SMOTE** or **undersampling** (not used here, but valuable in future enhancements).

### 3. Model Training
- Trained a **Random Forest Classifier** using default hyperparameters.
- Model trained on raw imbalanced data.

### 4. Evaluation Metrics
- **Confusion Matrix**
- **Precision / Recall / F1-Score**
- **ROC-AUC Curve**
- Focused on **minimizing false negatives** (failing to detect fraud).

---

## ✅ Results

> Note: Your exact results may vary based on random seed or train-test split.

- **Accuracy**: ~99.9% (but misleading due to imbalance)
- **Precision (fraud class)**: ~84%
- **Recall (fraud class)**: ~76%
- **F1-score (fraud class)**: ~80%
- **ROC-AUC**: ~0.97

⚠️ This highlights that traditional accuracy is not reliable for imbalanced datasets.

---

## 📌 Key Concepts

- Handling **class imbalance** in real-world datasets
- Using **Random Forests** for fraud detection
- Importance of **recall and precision** over accuracy
- Visualizing model performance (ROC curve, confusion matrix)

## 📁 File Structure

