# Awesome Video-Object-Detection

![Intro](https://github.com/ZHANGHeng19931123/seq_nms_yolo/raw/master/doc/intro1.gif "Intro")

This is a list of awesome articles about object detection from video.

## TODO

- [ ] Add summary for D&T
- [ ] Add summary for Scale-Time-Lattice
- [x] Add summary for STMN
- [x] Add summary for STSN
- [x] Add summary for MANet
- [ ] Add summary for Tracklet-Conditioned Detection

## Datasets

### ImageNet VID Challenge
- **Site**: http://image-net.org/challenges/LSVRC/2017/#vid
- **Kagge**: https://www.kaggle.com/account/login?returnUrl=%2Fc%2Fimagenet-object-detection-from-video-challenge

### VisDrone Challenge
- **Site**: http://aiskyeye.com/

## Paper list

### 2016

#### Seq-NMS for Video Object Detection

[[Arxiv]](https://arxiv.org/abs/1602.08465)

- **Date**: Feb 2016
- **Motivation**: Smoothing the final bounding box predictions across time.
- **Summary**:  Constructing a temporal graph from overlapping bounding box detections across the adjacent frames, and using dynamic programming to select bounding box sequences with the highest overall detection score.

#### T-CNN: Tubelets with Convolutional Neural Networks for Object Detection from Videos

[[Arxiv]](https://arxiv.org/abs/1604.02532) [[Code]](https://github.com/myfavouritekk/T-CNN)

- **Date**: Apr 2016
- **Summary**:  Using a video object detection pipeline that involves predicting optical flow first, then propagating image level predictions according to the flow, and finally using a tracking algorithm to select temporally consistent high confidence detections.
- **Performance**: 73.8% mAP on ImageNet VID validation.

#### Object Detection from Video Tubelets with Convolutional Neural Networks

[[Arxiv]](https://arxiv.org/abs/1604.04053) [[Code]](https://github.com/myfavouritekk/vdetlib)

- **Date**: Apr 2016

#### Deep Feature Flow for Video Recognition

[[Arxiv]](https://arxiv.org/abs/1611.07715) [[Code]](https://github.com/msracver/Deep-Feature-Flow)

- **Date**: Nov 2016
- **Performance**: 73.0% mAP on ImageNet VID validation at 29 fps on a Titan X GPU.

### 2017

#### Object Detection in Videos with Tubelet Proposal Networks

[[Arxiv]](https://arxiv.org/abs/1702.06355)

- **Date**: Feb 2017

#### Flow-Guided Feature Aggregation for Video Object Detection

[[Arxiv]](https://arxiv.org/abs/1703.10025) [[Code]](https://github.com/msracver/Flow-Guided-Feature-Aggregation)

- **Date**: Mar 2017
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 76.3% mAP at 1.4 fps or 78.4% (combined with [Seq-NMS](https://arxiv.org/abs/1602.08465)) at 1.1 fps on ImageNet VID validation on a Titan X GPU.

#### Detect to Track and Track to Detect

[[Arxiv]](https://arxiv.org/abs/1710.03958) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/X.md) [[Code]](https://github.com/feichtenhofer/Detect-Track)

- **Date**: Oct 2017
- **Motivation**: Smoothing the final bounding box predictions across time.
- **Summary**: Proposing a ConvNet architecture that solves detection and tracking problems jointly and applying a Viterbi algorithm to link the detections across time.
- **Performance**: 79.8% mAP on ImageNet VID validation.

#### Towards High Performance Video Object Detection

[[Arxiv]](https://arxiv.org/abs/1711.11577)

- **Date**: Nov 2017
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 78.6% mAP on ImageNet VID validation at 13 fps on a Titan X GPU.

#### Video Object Detection with an Aligned Spatial-Temporal Memory

[[Arxiv]](https://arxiv.org/abs/1712.06317) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/STMN.md) [[Code]](http://fanyix.cs.ucdavis.edu/project/stmn/project.html) [[Demo]](https://www.youtube.com/watch?v=Vs3LqY1s9GY)

- **Date**: Dec 2017
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 80.5% mAP on ImageNet VID validation.

### 2018

#### Object Detection in Videos by High Quality Object Linking

[[Arxiv]](https://arxiv.org/abs/1801.09823)

- **Date**: Jan 2018

#### Towards High Performance Video Object Detection for Mobiles 

[[Arxiv]](https://arxiv.org/abs/1804.05830)

- **Date**: Apr 2018
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 60.2% mAP on ImageNet VID validation at 25.6 fps on mobiles.

#### Optimizing Video Object Detection via a Scale-Time Lattice

[[Arxiv]](https://arxiv.org/abs/1804.05472) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/X.md) [[Code]](https://github.com/hellock/scale-time-lattice) 

- **Date**: Apr 2018
- **Performance**: 79.4% mAP at 20 fps or 79.0% at 62 fps on ImageNet VID validation on a Titan X GPU.

#### Object Detection in Video with Spatiotemporal Sampling Networks

[[Arxiv]](https://arxiv.org/abs/1803.05549) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/STSN.md)

- **Date**: Mar 2018
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 78.9% mAP or 80.4% (combined with [Seq-NMS](https://arxiv.org/abs/1602.08465)) on ImageNet VID validation.

#### Fully Motion-Aware Network for Video Object Detection

[[Paper]](http://openaccess.thecvf.com/content_ECCV_2018/html/Shiyao_Wang_Fully_Motion-Aware_Network_ECCV_2018_paper.html) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/MANet.md)

- **Date**: Stp. 2018
- **Motivation**: Producing powerful spatiotemporal features.
- **Performance**: 78.1% mAP or 80.3% (combined with [Seq-NMS](https://arxiv.org/abs/1602.08465)) on ImageNet VID validation.


#### Integrated Object Detection and Tracking with Tracklet-Conditioned Detection

[[Arxiv]](https://arxiv.org/abs/1811.11167) [[Summary]](https://github.com/ZHANGHeng19931123/awesome-video-object-detection/blob/master/X.md)

- **Date**: Nov 2018
- **Motivation**: Smoothing the final bounding box predictions across time.
- **Performance**: 83.5% of mAP with [FGFA](https://arxiv.org/abs/1703.10025) and [Deformable ConvNets v2](https://arxiv.org/abs/1811.11168) on ImageNet VID validation.

#### AdaScale: Towards Real-time Video Object Detection Using Adaptive Scaling
[[arXiv]](https://arxiv.org/pdf/1902.02910.pdf)
- Ting-Wu Chin et al., SysML 2019.

## Comparison table

| Paper | Date | Base detector | Backbone | Tracking? | Optical flow? | Online? | mAP(%) | FPS (Titan X) |
| ---|---| ---|---|---|---|---|---|---|
| [Seq-NMS](https://arxiv.org/abs/1602.08465) | Feb 2016 | [R-FCN](https://arxiv.org/abs/1605.06409) | ResNet101 | no | no | no | 76.8 | 2.3 |
| [T-CNN](https://arxiv.org/abs/1604.02532) | Apr 2016 | RCNN | DeepIDNet+CRAFT | yes | no | no | 73.8 | - |
| [DFF](https://arxiv.org/abs/1611.07715) | Nov 2016 | [R-FCN](https://arxiv.org/abs/1605.06409) | ResNet101 | no | yes | yes | 73.0 | 29 |
| [TPN](https://arxiv.org/abs/1702.06355) | Feb 2017 | TPN | GoogLeNet | yes | no | no | 68.4 | - |
| [FGFA](https://arxiv.org/abs/1703.10025) | Mar 2017 | [R-FCN](https://arxiv.org/abs/1605.06409) | ResNet101 | no | yes | yes | 76.3 | 1.4 |
| [FGFA](https://arxiv.org/abs/1703.10025) + [Seq-NMS](https://arxiv.org/abs/1602.08465) | 29 Mar 2017 | [R-FCN](https://arxiv.org/abs/1605.06409) | ResNet101 | no | yes | no | 78.4 | 1.14 |
| [D&T](https://arxiv.org/abs/1710.03958) | Oct 2017 | [R-FCN](https://arxiv.org/abs/1605.06409) (15 anchors) | ResNet101 | yes | no | no | 79.8 | 7.09 |
| [STMN](https://arxiv.org/abs/1712.06317) | Dec 2017 | [R-FCN](https://arxiv.org/abs/1605.06409) | ResNet101 | no | no | no | 80.5 | - |
| [Scale-time-lattice](https://arxiv.org/abs/1804.05472) | 16 Apr 2018 | [Faster RCNN](https://arxiv.org/abs/1506.01497) (15 anchors)| ResNet101 | no | no | no | 79.6 | 20 |
| [Scale-time-lattice](https://arxiv.org/abs/1804.05472) | Apr 2018 | [Faster RCNN](https://arxiv.org/abs/1506.01497) (15 anchors)| ResNet101 | no | no | no | 79.0 | **62** |
| [SSN](https://arxiv.org/abs/1803.05549) (per-frame baseline for STSN) | Mar 2018 | [R-FCN](https://arxiv.org/abs/1605.06409) | Deformable ResNet101 | no | no | yes | 76.0 | - |
| [STSN](https://arxiv.org/abs/1803.05549) | Mar 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| Deformable ResNet101 | no | no | yes | 78.9 | - |
| [STSN](https://arxiv.org/abs/1803.05549)+[Seq-NMS](https://arxiv.org/abs/1602.08465) | Mar 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| Deformable ResNet101 | no | no | no | 80.4 | - |
| [MANet](http://openaccess.thecvf.com/content_ECCV_2018/html/Shiyao_Wang_Fully_Motion-Aware_Network_ECCV_2018_paper.html) | Sep. 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| ResNet101 | no | yes | yes | 78.1 | 5 |
| [MANet](http://openaccess.thecvf.com/content_ECCV_2018/html/Shiyao_Wang_Fully_Motion-Aware_Network_ECCV_2018_paper.html)+[Seq-NMS](https://arxiv.org/abs/1602.08465) | Sep. 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| ResNet101 | no | yes | no | 80.3 | - |
| [Tracklet-Conditioned Detection](https://arxiv.org/abs/1811.11167) | Nov 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| ResNet101 | yes | no | yes | 78.1 | - |
| [Tracklet-Conditioned Detection](https://arxiv.org/abs/1811.11167)+[DCNv2](https://arxiv.org/abs/1811.11168) | Nov 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| ResNet101 | yes | no | yes | 82.0 | - |
| [Tracklet-Conditioned Detection](https://arxiv.org/abs/1811.11167)+[DCNv2](https://arxiv.org/abs/1811.11168)+[FGFA](https://arxiv.org/abs/1703.10025) | Nov 2018 | [R-FCN](https://arxiv.org/abs/1605.06409)| ResNet101 | yes | no | yes | **83.5** | - |
