# LINEAR-REGRESSION-WITH-PYTORCH

Python code used to study Linear Regression with Pytorch library and its use in Machine Learning.

![photo](https://raw.githubusercontent.com/ARBUCHELI/LINEAR-REGRESSION-WITH-PYTORCH/master/linearregresionwithpytorch.jpg)

Linear regression is one of the foundational algoritms of Machine Learning.  On this exercise I created a model that predicts crop yields for apples and oranges (target variables) by looking at input variables (average temperature, rainfall and humidity). In a region.

Here is the training Data:

    REGION        TEMP (F)    RAINFALL (mm)     HUMIDITY (%)      APPLES (ton)      ORANGES (ton)
    Texas         73          67                43                56                70  
    California    91          88                64                81                101
    Florida       87          134               58                119               133
    New Mexico    102         43                37                22                37
    Arizona       69          96                70                103               119

In a linear regression model, each target variable is estimated to be a weighted sum of the input variables, offset by some constant, known as a bias :

    yield_apple  = w11 * temp + w12 * rainfall + w13 * humidity + b1
    yield_orange = w21 * temp + w22 * rainfall + w23 * humidity + b2


Visually, it means that the yield of apples is a linear or planar function of temperature, rainfall and humidity:

![picture](https://i.imgur.com/4DJ9f8X.png)

The learning part of linear regression is to figure out a set of weights w11, w12,... w23, b1 & b2 by looking at the training data, to make accurate predictions for new data (i.e. to predict the yields for apples and oranges in a new region using the average temperature, rainfall and humidity). This is done by adjusting the weights slightly many times to make better predictions, using an optimization technique called gradient descent.

1. Type and run each line of code in [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb).
2. Or find the [original jupyter notebook](https://colab.research.google.com/gist/ARBUCHELI/3fd8eb4e231bdf5221dd786f05848925/linear-regression-with-pytorch.ipynb) and run the cells in Google Colab.


# Author: Andrés R. Bucheli.
(Inspired in Deep Learning with PyTorch - Zero to GANs - Udemy)
