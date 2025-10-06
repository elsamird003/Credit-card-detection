# Credit-card-detection#

This project uses **supervised machine learning** to detect fraudulent credit card transactions from an **imbalanced dataset** of over 284,000 records. The dataset is preprocessed, analyzed, and used to train a **Random Forest classifier**, with performance evaluated using relevant metrics like ROC-AUC and confusion matrix.

---

> Note: Your exact results may vary based on random seed or train-test split.
> <img width="861" height="450" alt="Screenshot 2025-10-05 at 7 29 39 PM" src="https://github.com/user-attachments/assets/0be3a906-c7b0-4efe-a99c-c22b04124439" />


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

