Detail Structure

I. Exploratory Data Analysis (EDA)
Statistical Figures: Display data types and descriptive statistics (mean, min, max, std)...
Imbalance Dataset Check: Visualize and quantify the class distribution (for this dataset: 34%/66% -> imbalanced ).
Feature Relationships and Correlation Matrix: Visualize the correlation matrix between all features to check for multicollinearity.

II. Training and Hyperparameter Tuning
Split the data and optimize our models using cross-validation.

Data Splitting:
Split the data into train and test.
Define 6-fold StratifiedKFold for cross-validation (cv).

Baseline Models (No Tuning):
Train and evaluate: GNB, LDA, QDA.

Hyperparameter Tuning (GridSearchCV):
Use GridSearchCV for optimization.
Tune: LogReg, DecTree, Bagging, XGBoost, RF, AdaBoost, GraBoost.

Stacking Ensemble:
Define base_learners: GNB, LDA, QDA
Define meta_learner: LogReg

III. Model Comparison and Reporting
Visualize results and select the best model.

Reporting:
Print the Final Test Results Table, sorted by CV Recall (highest priority metric).

Visualization:
Generate two separate, large box plots:
F2 Score: Train vs. Test scores from CV folds.
Recall: Train vs. Test scores from CV folds.
 
