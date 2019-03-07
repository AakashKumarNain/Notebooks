# Confusion Matrix

Confusion matrix is a NXN table that is used to evaluate the performance of a classifier.
It summarizes how successful a classification model's prediction were i.e. the correlation
between predictions and the grouth truth. 
Correct and Incorrect predictions are summarized with count values and broken down by each class. Implementing confusion matrix 
is straight forward. 

## Why this implementation when sklearn already comes with an implementation?
`sklearn` has no doubt a very robust implementation of confsuion matrix. The downside is that when you have more than two classes,
it doesn't provide the number of `TP`, `FP`, `TN` and `FN` for each class. This notebook aims to provide a method that can give the count for each category for each class


## Requirements:
* Python>=3.5
* numpy>=1.15
* matplotlib
