# Credit-Card-Fraud-Detection-Model
This project focuses on building **predictive machine learning models** to detect fraudulent transactions in credit card data. The dataset is highly **imbalanced**, with fraud cases making up just **0.172%** of all records. We experiment with multiple classification algorithms, analyze their performance, and explore techniquesto improve fraud detection. 
The models used include:

- **Random Forest Classifier**
- **AdaBoost Classifier**
- **CatBoost Classifier**
- **XGBoost**
- **LightGBM**

##Problem Statement

Credit card fraud detection is critical for financial institutions to reduce losses and protect customers. The key challenge is the extreme class imbalance — fraudulent transactions are rare but costly. The goal is to **identify these rare fraudulent transactions as accurately as possible**, minimizing both false positives and false negatives.

## Dataset
- **Transactions**: 284,807
- **Fraudulent cases**: 492 (0.172%)
- **Features**:
  - `V1` to `V28`: Principal Components (from PCA)
  - `Amount`: Transaction amount
  - `Time`: Time elapsed since the first transaction
  - `Class`: Target variable (1 = fraud, 0 = not fraud)

## ⚙️ Workflow Summary

### 1.Data Loading & Exploration
- Data imported and checked for nulls, imbalance, and distributions.
- Visual exploration of features using Seaborn and Plotly.

### 2.Data Preprocessing
- PCA-transformed data used directly.
- No categorical encoding needed.
- Feature `Amount` scaled where applicable.
- Dataset split into training and test sets using `train_test_split`.

### 3. Model Building
We trained and evaluated several models:
- **RandomForestClassifier** (with Gini as splitting criterion)
- **AdaBoostClassifier**
- **CatBoostClassifier** (handles categorical values natively)
- **XGBoost**
- **LightGBM**

  ###Model results
  **RandomForestClassifier**(ROU-AUC SCORE=0.8528641975628091)
  **AdaBoostClassifier**(ROU-AUC SCORE=0.8332343604519027)
  **CatBoostClassifier**(ROU-AUC SCORE=0.8577991493075996)
  **XGBoost**(ROU-AUC SCORE=0.9777955400794907)
  **LightGBM**(ROU-AUC SCORE=0.9473337202349548)
  

