# fraud-detection-using-machine-learning
End-to-end fraud detection project applying PCA, k-NN, Random Forest, and clustering techniques to identify fraudulent credit card transactions with high precision and recall.
📌 Credit Card Fraud Detection Using Machine Learning
🧠 Project Overview

This project focuses on detecting fraudulent credit card transactions using a combination of supervised and unsupervised machine learning techniques. Due to the extreme class imbalance (fraud rate ~0.17%), special attention is given to evaluation metrics such as Precision, Recall, F1-score, and PR-AUC rather than accuracy.

The solution integrates predictive modeling with anomaly detection to provide a robust, real-world fraud detection framework suitable for financial institutions.

🎯 Business Problem

Financial fraud causes significant monetary loss and customer dissatisfaction. The goal of this project is to:

Maximize fraud detection (Recall)

Minimize false alerts (Precision)

Support operational decision-making through risk segmentation

📊 Dataset

Source: Kaggle – Credit Card Fraud Detection Dataset (2018)

Records: 284,807 transactions

Fraud Rate: 0.172%

Features:

Time, Amount

28 PCA-transformed anonymized features

Target: Class (1 = Fraud, 0 = Legitimate)

🛠️ Techniques & Models Used

Supervised Learning

Decision Tree

Random Forest

Support Vector Machine (RBF Kernel)

k-Nearest Neighbors (k-NN)

Unsupervised Learning

K-Means Clustering (Risk Segmentation)

Preprocessing

Standard Scaling

PCA (20 components)

SMOTE & Class Weighting

🏆 Model Performance Summary
Model	Precision	Recall	F1-Score	PR-AUC
Decision Tree	88.24%	70.41%	78.24%	81.00%
Random Forest	91.57%	77.55%	83.98%	84.83%
SVM (RBF + PCA)	89.40%	73.00%	80.10%	83.20%
k-NN (k=5, PCA20)	94.05%	80.61%	86.81%	85.50%

✅ Best Model: k-NN with PCA

📈 Key Insights

PCA improved local neighborhood structure, enabling k-NN to outperform tree-based models.

Random Forest provided strong generalization and interpretability.

K-Means clustering revealed high-risk transaction groups useful for alert prioritization.

Hybrid supervised + unsupervised approach improved fraud triage effectiveness.

🚀 Business Impact

Reduced fraud losses through higher recall

Lower false positives → improved customer experience

Efficient alert prioritization for fraud analysts

🔮 Future Enhancements

Autoencoders & LSTM for sequential fraud detection

Real-time fraud scoring pipelines

SHAP/LIME for explainability

Model drift monitoring

📎 Files in This Repository

notebooks/ – Model implementation

reports/ – Detailed project report

images/ – Visualizations & results

👤 Author

Gourang Chauhan
Graduate Student – Business Analytics
Machine Learning | Data Analytics | Fraud Detection

