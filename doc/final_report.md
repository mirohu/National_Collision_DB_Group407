Predicting Car Crash Fatalities and Proposing Solutions to Save Lives
================

## Summary:

Here we attempt to build a classification model using a variety of
different machine learning algorithms to distinguish between fatal and
non-fatal car accidents based on a set of relevant features. Our best
model gave us a recall and precision score of X and Y respectively.

## Introduction:

It is quite unfortunate that every year thousands of Canadians die from
health-related problems such as cancer and disease. However, based
purely on a statistical odds it is more likely for an individual to die
from a car accident. In 2017, over 150,000 individuals faced a car
collision with over 1,800 unfortunately resulting in fatalities
(Government of Canada, 2017).

We want to harness the power machine learning to a rich dataset of car
collision statistics to see if we can determine whether an accident will
result in a fatality or not. By better understanding the predictive
features which cause fatal accidents we can help inform policy makers to
implement meaningful change and help save lives.

## Methods:

### Data:

The data we are using is from the National Collision Database and can be
found on the Government of Canada website. It’s a database that contains
all police-reported motor vehicle collisions on public roads in Canada.
The data we specifically chose was from 2017. Each row provides several
data points for a passenger with the detailed summary statistics of the
collision. Analysis:

We applied several classification models including: Logistic Regression
and the Random Forest Classifier. None of the data points in our dataset
contained continuous variables as all of the values were discrete. For
this reason, we were required to create dummy variables for each of the
classes in each column to prevent our model from learning false
relationships within the data. As an example, in the original dataset
the `C_WDAY` has 7 different values ranging from 1 to 7. In this case,
it is not appropriate to assert that day 4 is of greater importance than
day 2, however, the machine learning model will pickup on this inherent
relationship.

We used the Python programming language (Van Rossum and Drake 2009),
Pandas library (McKinney 2010) and Scikit-Learn library (David
Cournapeau, 2007) to wrangle data and perform the machine learning
analysis.

### Results and Discussion:

Accuracy is not an appropriate measure to include for our analysis here
because the data is highly imbalanced. Virtually any classification
model can achieve high accuracy when the data is highly imbalanced,
however, the primary metric is precision and recall. Overall we found
that the Random Forest classification model performed the best with the
highest overall recall and precision of Xand Y respectively based on the
confusion
matrix.

### \>\> Insert chart and image of random forest + Logistic Regression (reference it from the results folder).

As a whole we believe there are further improvements that can be made in
future iterations of this project. Firstly, we believe that using more
data from previous years can help us better learn any temporal
relationships and seasonality which may be present. Furthermore, our
current analysis was not implemented with hyper parameter optimization
but for the future we would want to tweak our model accordingly to
refining the overall predictive capacity of our model.

References: