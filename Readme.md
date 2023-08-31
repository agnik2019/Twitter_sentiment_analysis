## Twitter Sentiment Analysis

### Data Analysis
Size of training dataset =  8001 

Size of validation dataset = 1380

Size of test dataset = 3136

Average text length of the tweets (in training dataset) 19.63

| Sentiment              | Count  |
|------------------------|--------|
| Positive               | 2973   |
| Neutral                | 1446   |
| Objective-OR-Neutral   | 1391   |
| Negative               | 1159   |
| Objective              | 1032   |

### Feature Engineering
I have used tfidf vectorizer as tokenizer for the machine learning models. Also, I have used tokenizer of bert-base-uncased for tokenizing the text for deep learning model.
### Modelling
I have used Machine learning models such as Logistic Regression, Support vector machines, Random forest classifier and multinomial naive bayes. I have used gridSearchCv for trying out different parameters and to get best params. The code snippet is available on `tweet_classify_ml_model.ipynb` file.

I have used pre-trained model bert-base-uncased. The hyperparameters are learning_rate=1e-5, epochs = 3, loss = Sparse Categorical Crossentropy. The bert model's code snippet is available on `tweet_classify_deep_model.ipynb` file.

### Evaluation
Following table contains Model name and its accuracy on the validation set.

| Model                              | Accuracy      |
| -----------------------------------| ------------- |
|Logistic Regression               |   0.63         |
|Support Vector Machine           |   0.64         |
|Random Forest Classifier | 0.602|                                
| Multinomial Naive Bayes|  0.615 |
| Bert|  0.74 |

So from this experiment it has been observed that Bert achieves high accuracy.


