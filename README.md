Some data science projects I have worked on.

## Fraud Detection
With data obtained from Kaggle, XGBoost and cross-validation, I created a model that can predict when credit card fraud has occurred with a test set F1-score of 0.88. Since
the majority of data points are non-fraud, accuracy is a poor measure of how well a model can predict fraud occurrence. So average precision and F1-scores were used as
model evaluation metrics instead. A boosted classification forest was fit using XGBoost, and its parameters were selected with a Scikit-learn grid search with an average 
precision scoring metric. Then a probability threshold was selected using Scikit-learn's tuned threshold cross-validation to find the threshold which resulted in the best 
validation set F1-score. The Jupyter notebook titled fraud_detection holds all of the code.

## Shakespeare Generation with a Character Level RNN
I used a LSTM RNN to generate Shakespeare-like text by predicting the next character in a sequence of characters. The model can generate actual words and use punctuation, but the text
doesn't make sense overall. And it still makes up some words. But I think it's not bad for its size/limitations. The Jupyter notebook titled Shakespeare_RNN holds the model and some text it generated after training.
