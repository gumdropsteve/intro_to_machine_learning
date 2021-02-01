# Logistic Regression and Gradient Descent
Slides: https://docs.google.com/presentation/d/14gGuib92IjgNtB6t2rwTOZRRYAx0h8742JchORNVdBw/edit?usp=sharing

#### Logistic Regression
> Essentially, the logistic regression function takes examples with known classes (e.g. cake (1) or pie (0)), fits a (Sigmoid) line to their distribution, and makes calculated guesses as to which class future examples (with unknown classes) fall into. - [Winston Robson](https://medium.com/dropout-analytics/beginners-guide-to-logistic-regression-with-cuml-5061086d8694?source=friends_link&sk=2d8d0f7ddd43ccaaf264afcbadeea231)

![https://medium.com/dropout-analytics/beginners-guide-to-logistic-regression-with-cuml-5061086d8694](https://miro.medium.com/max/434/1*o3Az8VY4znWBJbN95Q9TyA.png)

> In statistics, the logistic model (or logit model) is used to model the probability of a certain class or event existing such as pass/fail, win/lose, alive/dead or healthy/sick. This can be extended to model several classes of events such as determining whether an image contains a cat, dog, lion, etc. Each object being detected in the image would be assigned a probability between 0 and 1, with a sum of one. - [Wikipedia](https://en.wikipedia.org/wiki/Logistic_regression)


#### Gradient Descent
> Gradient descent is a first-order iterative optimization algorithm for finding a local minimum of a differentiable function. The idea is to take repeated steps in the opposite direction of the gradient (or approximate gradient) of the function at the current point, because this is the direction of steepest descent. Conversely, stepping in the direction of the gradient will lead to a local maximum of that function; the procedure is then known as gradient ascent. - [Wikipedia](https://en.wikipedia.org/wiki/Gradient_descent)

> Gradient descent is an optimization algorithm used to minimize some function by iteratively moving in the direction of steepest descent as defined by the negative of the gradient. In machine learning, we use gradient descent to update the parameters of our model. Parameters refer to coefficients in Linear Regression and weights in neural networks. - [ML Glossary](https://ml-cheatsheet.readthedocs.io/en/latest/gradient_descent.html)

![](https://ml-cheatsheet.readthedocs.io/en/latest/_images/gradient_descent_demystified.png)

## Resources
#### API Reference
- sklearn.linear_model.LogisticRegression: 
  - Docs: [scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) 
  - Source Code: [github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_logistic.py#L1012](https://github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_logistic.py#L1012)
- sklearn.linear_model.SGDClassifier:
  - Docs [scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDClassifier.html](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDClassifier.html)
  - Source Code: [github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_stochastic_gradient.py#L735](https://github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_stochastic_gradient.py#L735)

#### Readings
- Beginner’s Guide to Logistic Regression with cuML: [medium.com/dropout-analytics/beginners-guide-to-logistic-regression-with-cuml-5061086d8694?source=friends_link&sk=2d8d0f7ddd43ccaaf264afcbadeea231](https://medium.com/dropout-analytics/beginners-guide-to-logistic-regression-with-cuml-5061086d8694?source=friends_link&sk=2d8d0f7ddd43ccaaf264afcbadeea231)
- Grid search or gradient descent?: [datascience.stackexchange.com/questions/62323/grid-search-or-gradient-descent](https://datascience.stackexchange.com/questions/62323/grid-search-or-gradient-descent)

#### Sklearn Stuff
- Scikit Learn Cheat Sheet (Python): [github.com/daniel-dc-cd/data_science/blob/master/module_4_ML/Linear%20Regression/Scikit_Learn_Cheat_Sheet_Python.pdf](https://github.com/daniel-dc-cd/data_science/blob/master/module_4_ML/Linear%20Regression/Scikit_Learn_Cheat_Sheet_Python.pdf)
- (Release) scikit-learn 0.24.1: [github.com/scikit-learn/scikit-learn/releases/tag/0.24.1](https://github.com/scikit-learn/scikit-learn/releases/tag/0.24.1)

#### Videos
- StatQuest: Logistic Regression: [youtu.be/yIYKR4sgzI8](https://youtu.be/yIYKR4sgzI8)
- Gradient Descent, Step-by-Step: [youtu.be/sDv4f4s2SB8](https://youtu.be/sDv4f4s2SB8)
