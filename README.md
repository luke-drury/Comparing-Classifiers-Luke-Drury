Comparing Classifiers

**Goal.** Compare KNN, Logistic Regression, Decision Tree, and SVM to predict whether a client will subscribe to a term deposit.

**Data.** UCI Bank Marketing dataset (Portuguese bank). CSVs use `;` as delimiter.

**Method.**
- Clean + encode features with a `ColumnTransformer` (scale numerics, one-hot categoricals).
- Stratified train/test split; 5-fold CV with small grids for speed.
- Metrics: Accuracy, F1, ROC-AUC (F1/ROC-AUC emphasized due to class imbalance).

**Results.**
- Best model (by F1): SVC_RBF (see notebook for details, confusion matrix, ROC/PR curves, and coefficients if logistic).

**How to run.**
1) Put CSV or ZIP in `data/` (or notebook root).
2) Open the notebook and run all cells.

**References.**
- UCI Machine Learning Repository: Bank Marketing dataset.
- scikit-learn, pandas, seaborn, matplotlib docs.


