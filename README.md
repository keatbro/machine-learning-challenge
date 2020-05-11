# machine-learning-challenge

The purpose of this challenge was to analyze a dataset from NASA's Kepler space telescope and use machine learning to classify observed candidate exoplanets.

### Preprocessing

The dataset used was fairly large (41 columns), so in order to minimize potential bias from including unnecessary fields, I used the f_classif method to calculate ANOVA F-values for each field and chose the features with the eight-heightest values. (There was a noticeable difference in F-Value between the 8th & 9th value).

### Models

Two models were used in this analysis, a Random Forest model (random_forest.ipynb), and a Support Vector Machine (svm.ipynb) model. Both models produced fairly consistent results on the test data (R-squared values of 0.821 and 0.816 for the RF and SVM models, respectively). Copies of the models are also saved in their respective .sav files. I used GridSearchCV to adjust the model parameters for models, and this produced a slightly greater effect for the RF Model (score of 0.844) than it did the SVM model (0.820).

