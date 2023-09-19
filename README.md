# Essay-Scoring-Model-using-NLP

This is a machine learning project to build a model that can automatically score student essays on a scale from 1 to 12. The data consists of text samples from student essays along with human-assigned scores.

**Data**
The training data is in IMT575_HW3_train.tsv and the test data is in IMT575_HW3_test.tsv. Both files have two columns - score and text.

score - the human assigned score for the essay (1-12)
text - the text content of the essay

**Models**
The following models are implemented and evaluated:

-Ridge regression
-Ridge regression with sentiment feature
-SVR
-SVR with sentiment feature
-SVR with sentence embeddings from Universal Sentence Encoder
-Grid search is used to tune the hyperparameters of each model.

**Evaluation**
The models are evaluated using mean squared error (MSE) on the test set. Lower MSE indicates better performance.

**Results**
The SVR model with grid search performed the best with a test MSE of 0.7845. Adding sentiment features provided minor improvements for both Ridge and SVR models. The sentence embedding model did not perform as well as expected compared to bag-of-words models
