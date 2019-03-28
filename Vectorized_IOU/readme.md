# Vectorized implementation of IOU for bounding boxes

## What is Intersection over Uniona(aka IOU)?
Intersect over Union (IoU) is a metric that allows us to evaluate how similar our predicted bounding box is to the ground truth bounding box. The idea is that we want to compare the ratio of the area where the two boxes overlap to the total combined area of the two boxes. 

``` math
IOU = Intersecting Area of two bounding boxes / Union of Areas of the two boxes
```
