# Object Detection in Video with Spatiotemporal Sampling Networks

## Architecture

![](imgs/STSN.png)

## Summary

Using [deformable convolutions](https://arxiv.org/abs/1703.06211)  across space and time (instead of optical flow) to leverage temporal information for object detection in video, i.e., using **deformable convolutions** to sample relevant features from nearby frames (27 frames in total) and using **temporally aggregagtion** (per-pixel weighted summation) to generate final feature maps for detection network ([R-FCN](https://arxiv.org/abs/1605.06409)).
