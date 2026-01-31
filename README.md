💳 Credit Card Fraud Detection

Overview
Machine learning project for detecting fraudulent credit card transactions.
The dataset is highly imbalanced (fraud < 1%), so the focus is on recall and F1-score, not accuracy.

Dataset
Kaggle Credit Card Fraud Dataset

~284K transactions

Features: V1–V28 (PCA), Amount

Target:

0 → Normal

1 → Fraud

Approach
Exploratory Data Analysis to understand class imbalance

Memory optimization and feature scaling

Logistic Regression with class_weight='balanced'

Hyperparameter tuning using GridSearchCV

Threshold tuning to improve fraud detection

Evaluation
Confusion Matrix

Precision, Recall, F1-score

ROC Curve & AUC

Accuracy was avoided due to extreme class imbalance.

Results
Detects ~92–96% of fraud transactions depending on the threshold

Lower thresholds increase fraud recall with more false positives

Key Takeaways
Problem understanding matters more than complex models

Threshold tuning is critical in fraud detection

Logistic Regression is a strong and interpretable baseline

Tools
Python, Pandas, Seaborn, Matplotlib, Scikit-learn

Author
Ameen Nasairah
