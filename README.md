
# 💳 Credit Card Fraud Detection

This project focuses on building a machine learning model to detect fraudulent transactions in credit card data. Fraud detection is a critical use case in financial security, where timely and accurate identification of fraud can save millions in losses.

---

## 📌 Project Overview

**Goal:**  
Detect fraudulent credit card transactions using supervised machine learning algorithms.

**Dataset:**  
- Publicly available dataset containing transactions made by European cardholders in September 2013.
- The dataset is highly imbalanced, with only a small fraction of transactions being fraudulent.

**Key Features:**
- Features are numerical, result of PCA transformation.
- `Time`, `Amount`, and `Class` (0 = Legitimate, 1 = Fraud) are retained in raw form.

---

## 🛠️ Workflow

1. **Data Preprocessing**
   - Handling imbalance using techniques like under-sampling or SMOTE (if used).
   - Feature scaling for models sensitive to input magnitude.

2. **Exploratory Data Analysis (EDA)**
   - Distribution of legitimate vs. fraudulent transactions.
   - Correlation heatmaps to inspect feature relationships.

3. **Model Building**
   - Machine learning model trained (e.g., Logistic Regression, Random Forest, or others as per notebook).
   - Split into training and testing sets using stratified sampling.

4. **Model Evaluation**
   - Accuracy, Precision, Recall, F1-Score, and AUC-ROC.
   - Confusion matrix and ROC curve for performance visualization.

---

## 📊 Results

- **Training Accuracy:** 95%  
- **Test Accuracy:** 91%  
- **Precision/Recall:** Optimized to prioritize fraud detection even in imbalanced scenarios.

---

## 🔍 Key Insights

- Fraudulent transactions were successfully identified with high accuracy.
- The model generalizes well to unseen data, with a 4% drop between training and testing accuracy—indicating minimal overfitting.
- Additional metrics like precision and recall (especially recall for fraud cases) should be monitored closely in deployment.

---

## 🚀 Future Work

- Implement real-time detection using streaming data pipelines.
- Integrate with APIs for production deployment.
- Explore ensemble models and anomaly detection techniques for improved robustness.

