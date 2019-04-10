# Quadratic Weighted Kappa 

Quadratic weighted kappa, which measures the agreement between two ratings. This metric typically varies from `0` (random agreement between raters) to `1` (complete agreement between raters). In the event that there is less agreement between the raters than expected by chance, the metric may go below `0`. The quadratic weighted kappa is calculated between the scores which are expected/known and the predicted scores.

# Why Quadratic Kappa and not simple Kappa score?
Quadratic Kappa allows you to weight the disagreements differently. It is especially useful when the categories are ordered. For example, suppose the groundth truth is `1`. Now let's say that the rating are on a scale of `1` to `5`. If the rater rates it as `5`, then the penalty would be much higher as compared to if the rater rates it as `2`

# How does it calculated?

`Weighted Kappa` calculation involves three matrices namely:
* `O`: NxN normalized confusion matrix, denoting the observed agreement
* `W`: NxN Weight matrix
* `E`: NxN normalized expected matrix

