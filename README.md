Credit Risk Prediction Project

This project aims to predict clients’ credit risk using various machine learning algorithms.
Three models were tested — Decision Tree, Random Forest, and XGBoost — with XGBoost achieving the best results based on the AUC metric.

The goal of the project is to classify clients as risky or non-risky based on their financial characteristics.
The model is intended to assist financial institutions in making informed decisions about loan approvals.

If the model returns 0, the client is very likely to repay the loan, and the bank may approve it.

If the model returns 1, the client is considered a potential defaulter, and the bank may decide not to approve the loan.

Dataset

The dataset used in this project is available [here](https://github.com/gastonstat/CreditScoring).

Model Tuning and Results

Model hyperparameters were tuned manually by testing different parameter combinations and evaluating them using the ROC-AUC curve.

Decision Tree: achieved an AUC score of 0.805 on the validation set.

Random Forest: achieved an AUC score of 0.8383 on the validation set.

XGBoost: achieved an AUC score of 0.8475 on the validation set.

Since XGBoost provided the highest AUC score, it was selected as the final model.
When evaluated on the test set, it achieved an AUC score of 0.84, indicating no overfitting and model stability.
