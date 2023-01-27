# Naive Bayes

## When to Use Naive Bayes

Because naive Bayesian classifiers make such stringent assumptions about data, they will generally not perform as well as a more complicated model.
Advantages:

- They are extremely fast for both training and prediction
- They provide straightforward probabilistic prediction
- They are often very easily interpretable
- They have very few (if any) tunable parameters

These advantages mean a naive Bayesian classifier is often a good choice as an initial baseline classification.
If it performs suitably, then congratulations: you have a very fast, very interpretable classifier for your problem.
If it does not perform well, then you can begin exploring more sophisticated models, with some baseline knowledge of how well they should perform.

Naive Bayes classifiers tend to perform especially well in one of the following situations:

- When the naive assumptions actually match the data (very rare in practice)
- For very well-separated categories, when model complexity is less important
- For very high-dimensional data, when model complexity is less important

The last two points seem distinct, but they actually are related: as the dimension of a dataset grows, it is much less likely for any two points to be found close together (after all, they must be close in *every single dimension* to be close overall).
This means that clusters in high dimensions tend to be more separated, on average, than clusters in low dimensions, assuming the new dimensions actually add information.
For this reason, simplistic classifiers like naive Bayes tend to work as well or better than more complicated classifiers as the dimensionality grows: once you have enough data, even a simple model can be very powerful.


## Implementation

<img src="NB/img/NB1.JPG" height="300" width="400">  | <img src="NB/img/NB2.JPG" height="300" width="400">
------------- | -------------
<img src="NB/img/NB3.JPG" height="300" width="400">  | 
<img src="NB/img/NB4.JPG" height="300" width="400">   | <img src="NB/img/NB5.JPG" height="300" width="400">
   | <img src="NB/img/NB6.JPG" height="300" width="400">
<img src="NB/img/NB7.JPG" height="300" width="400">   | <img src="NB/img/NB8.JPG" height="300" width="400">
<img src="NB/img/NB9.JPG" height="300" width="400">   | <img src="NB/img/NB10.JPG" height="300" width="400">
<img src="NB/img/NB11.JPG" height="300" width="400">   | <img src="NB/img/NB12.JPG" height="300" width="400">
<img src="NB/img/nb13.JPG" height="300" width="400">   | 

<img src="NB/img/NB14.JPG" height="300" width="400">  |
<img src="NB/img/NB15.JPG" height="300" width="400">   | <img src="NB/img/NB16.JPG" height="300" width="400">
<img src="NB/img/NB17.JPG" height="300" width="400">   | <img src="NB/img/NB18.JPG" height="300" width="400">
<img src="NB/img/nb19.JPG" height="300" width="400">   | <img src="NB/img/NB20.JPG" height="300" width="400">
<img src="NB/img/NB21.JPG" height="300" width="400">   | <img src="NB/img/nb22.JPG" height="300" width="400">
<img src="NB/img/NB23.JPG" height="300" width="400">
