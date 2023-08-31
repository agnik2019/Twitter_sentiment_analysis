## Twitter Sentiment Analysis

### Dataset description
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

### Model description
Following table contains Model name and its accuracy on the validation set.

| Model                              | Accuracy      |
| -----------------------------------| ------------- |
|Logistic Regression               |   0.63         |
|Support Vector Machine           |   0.64         |
|Random Forest Classifier | 0.602|                                
| Multinomial Naive Bayes|  0.615 |
| Bert|  0.74 |

So from this experiment it has been seen that Bert achieves high accuracy.
I have used pre-trained tokenizer as well as model bert-base-uncased.


