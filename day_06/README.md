# Linear Regression & Gradient Descent
#### Linear Regression
> In statistics, linear regression is a linear approach to modelling the relationship between a scalar response and one or more explanatory variables (also known as dependent and independent variables). The case of one explanatory variable is called simple linear regression; for more than one, the process is called multiple linear regression. This term is distinct from multivariate linear regression, where multiple correlated dependent variables are predicted, rather than a single scalar variable. - [Wikipedia](https://en.wikipedia.org/wiki/Linear_regression)

![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Linear_regression.svg/440px-Linear_regression.svg.png)

> Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. One variable is considered to be an explanatory variable, and the other is considered to be a dependent variable. For example, a modeler might want to relate the weights of individuals to their heights using a linear regression model. - [Yale](http://www.stat.yale.edu/Courses/1997-98/101/linreg.htm)

#### Gradient Descent
> Gradient descent is a first-order iterative optimization algorithm for finding a local minimum of a differentiable function. The idea is to take repeated steps in the opposite direction of the gradient (or approximate gradient) of the function at the current point, because this is the direction of steepest descent. Conversely, stepping in the direction of the gradient will lead to a local maximum of that function; the procedure is then known as gradient ascent. - [Wikipedia](https://en.wikipedia.org/wiki/Gradient_descent)

> Gradient descent is an optimization algorithm used to minimize some function by iteratively moving in the direction of steepest descent as defined by the negative of the gradient. In machine learning, we use gradient descent to update the parameters of our model. Parameters refer to coefficients in Linear Regression and weights in neural networks. - [ML Glossary](https://ml-cheatsheet.readthedocs.io/en/latest/gradient_descent.html)

![](https://ml-cheatsheet.readthedocs.io/en/latest/_images/gradient_descent_demystified.png)

## Resources
#### API Reference
- sklearn.linear_model.LinearRegression: 
  - Docs: [scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html) 
  - Source Code: [github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_base.py](https://github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_base.py#L391)
- sklearn.linear_model.SGDRegressor:
  - Docs [scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDRegressor.html](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDRegressor.html)
  - Source Code: [github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_stochastic_gradient.py](https://github.com/scikit-learn/scikit-learn/blob/b3ea3ed6a/sklearn/linear_model/_stochastic_gradient.py#L1366)

#### Readings
- Beginner’s Guide to Linear Regression with cuML: [medium.com/future-vision/beginners-guide-to-linear-regression-in-python-with-cuml-30e2709c761](https://medium.com/future-vision/beginners-guide-to-linear-regression-in-python-with-cuml-30e2709c761?source=friends_link&sk=1da35920b9e2ffea59d5cb3c998bfeae)
- In Depth: Linear Regression: [jakevdp.github.io/PythonDataScienceHandbook/05.06-linear-regression.html](https://jakevdp.github.io/PythonDataScienceHandbook/05.06-linear-regression.html)
- Grid search or gradient descent?: [datascience.stackexchange.com/questions/62323/grid-search-or-gradient-descent](https://datascience.stackexchange.com/questions/62323/grid-search-or-gradient-descent)

#### Videos
- StatQuest: Linear Models Pt.1 - Linear Regression: [youtu.be/nk2CQITm_eo](https://youtu.be/nk2CQITm_eo)
- StatQuest: Linear Models Pt.1.5 - Multiple Regression: [youtu.be/zITIFTsivN8](https://youtu.be/zITIFTsivN8)
- Gradient Descent, Step-by-Step: [youtu.be/sDv4f4s2SB8](https://youtu.be/sDv4f4s2SB8)
