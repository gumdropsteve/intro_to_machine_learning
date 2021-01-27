# Model Evaluation
After you have built a model using iterative improvement techniques (gradient descent) it is important to evaluate its quality. The method of determining model quality is commonly referred to as cross validation. The most common method of cross validation is to first (before training the model) break the data set into two pieces, training and testing.
- Training dataset ~ 80% of the total dataset
- Testing dataset ~ 20% of the total dataset

The actual break down between training and testing can vary depending on the needs of the project or the availability of data. There is a very handy function built into scikit-learn that will perform this subsetting.

```python
from sklearn.model_selection import train_test_split 
X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0) 
```

Once the dataset is broken down then the model is built against the training set. The intuition is that if you hold out a set of features and realizations from the training set you can see how the model will perform against data it has never seen before. 

The test set works as a control against overfitting.  Overfitting is the concept of fitting a model too tightly with its realizations. In fact, it is possible to construct models that exactly fit the historical data. However, such models then perform very badly against data not used during training. 

The performance of the model is measured in two ways. How well the model fits the training data and the difference between the model's performance on the training and test set. These two performance metrics are called bias and variance:
- bias: poor performance on the training data
- variance: a large difference between training model performance and test set performance

![](https://lh6.googleusercontent.com/20YsbCrQM_jtD99EoHVrcFp54FqhraTeyJmQYN4qVLqt7jG5aShnT0dr44Ss2lcdI3iCOg_Z_JHwsvbi77VT5A0JIlAxdtmM90koEGKJNFisoOdmoRXejzTeL0XDCgpwQbyffOk)

There are many measures of quality when fitting models. Those that are fit to continuous real numbers (for example a price, time or size) quality can be expressed as the value of the cost function or some correlation metric like R^2 ([information on this topic here](https://en.wikipedia.org/wiki/Coefficient_of_determination)). 

With classification models there are some more intuitive methods. One set of measures for these models is accuracy, precision and recall, which are percentages of certain types of quality as shown in the figure here ([source](https://en.wikipedia.org/wiki/Precision_and_recall)).

![](https://lh5.googleusercontent.com/D0a1Uu_b4ApyzJX4FkU20IfksuRfVDd7AKzcezmi03O_mJAHrwf925VVXIScGg6J-_bH3yROIkR3z8R1F2-pcjSXmR7NvF10169uvqYRo70tz8yR-emiDjkaA5CKn38fZ_2qRo8)

The four concepts of true/false negative/positive are measures of your guesses 
- Precision: The percent of the time you predict positive that you are correct
- Recall: The percentage of positive guesses you got correct that you should have gotten correct

These values then serve as a core measure of performance. This information can also be organized using a [confusion matrix](https://en.wikipedia.org/wiki/Confusion_matrix):

![](https://lh5.googleusercontent.com/P5H1wOfDy7bw8T75tSiJMybXngiiVtKYKGzB3R_YwH3JnytMwYlDGcQzw1yIC0JHKbl6rfgJUgQQ8Qia-FrHMkCjIvfK6_haxIzLndw-Glcrx3RV2Ay2vz7F78l3z8L7xy3bRng)

## Resources
- Readings
  - [05.02-Introducing-Scikit-Learn.ipynb](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.02-Introducing-Scikit-Learn.ipynb)
  - [05.03-Hyperparameters-and-Model-Validation.ipynb](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.03-Hyperparameters-and-Model-Validation.ipynb)
- Videos
  - StatQuest: [Machine Learning Fundamentals: Cross Validation](https://youtu.be/fSytzGwwBVw)
  - StatQuest: [Machine Learning Fundamentals: The Confusion Matrix](https://youtu.be/Kdsp6soqA7o)
  - StatQuest: [Machine Learning Fundamentals: Bias and Variance](https://youtu.be/EuBBz3bI-aA)
  - Machine Learning (YouTube playlist): [youtube.com/watch?v=Gv9_4yMHFhI&list=PLblh5JKOoLUICTaGLRoHQDuF_7q2GfuJF](https://www.youtube.com/watch?v=Gv9_4yMHFhI&list=PLblh5JKOoLUICTaGLRoHQDuF_7q2GfuJF)
