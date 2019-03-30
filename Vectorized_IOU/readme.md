# Vectorized implementation of IOU for bounding boxes

## What is Intersection over Uniona(aka IOU)?
Intersect over Union (IoU) is a metric that allows us to evaluate how similar our predicted bounding box is to the ground truth bounding box. The idea is that we want to compare the ratio of the area where the two boxes overlap to the total combined area of the two boxes. 

![alt text](./iou_equation.png)

## Why this implementation?
IOU is an important metric for many types of models. It is heavily used in Object detection. Computing IOU for each pair(groundtruth and prediction) can be expensive if you are using a `for` loop. What we really want is a vectorized implementation so that we can computer the IOU in a single pass
