# Assignment 2 - Notes

_Accuracy_ of a classifier = sum of correctly classified elements divided by the sum of all elements. With numpy we can do a nifty trick `(y_predict == y_label).mean()`.

One dimensional vectors in `numpy`, so arrays of shape `(N, )` are neither column nor row vectors. To be a row vector, it must have shape `(1, N)` or for a column vector it's `(N, 1)`.
