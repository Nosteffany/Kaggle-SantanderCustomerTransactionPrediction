# Kaggle-SantanderCustomerTransactionPrediction
Deal with highly imballanced dataset and, as it turned out, with fake samples in train and test set

Tried several techniques like:
  1. Simple XGBClassifier with Grid and Random search. Then they were replaced by a Bayesian optimizer(Hyperopt)
  2. Undersampling by reducing the majority class.
  3. Oversampling methods like SMOTE, ADASYN and SMOTE+ENN. Tested with XGBoost.
  4. Catboost
  5. Catboost + Recurent Feature Elimination technique


SUBMISIONS

1) Score: 0.82182 --- Xgboost + Hyperopt + Undersampling 	(Part of train data)
2) Score: 0.85069 --- Simple LogisticRegression			      (Part of train data)
6) Score: 0.86523 --- Xgboost + Hyperopt 			            (Part of train data)
7) Score: 0.84935 --- LogisticRegression(class weight)		(Part of train data)
8) Score: 0.85841 --- Xgboost(scale weight)			          (Part of train data)
9) Score: 0.87805 --- Xgboost + Hyperopt			            (All train data)
10) Score: 0.83289 --- DenseNN					                  (Part of train data)
11) Score: 0.89381 --- CatBoost only				              (All train data)
12) Score: 0.88999 --- CatBoost + RFE			              	(All train data)

3,4,5 skipped due their poor scores. (Oversampling techniques)
