# Awesome Video-Object-Detection

![Intro](https://github.com/ZHANGHeng19931123/seq_nms_yolo/raw/master/doc/intro1.gif "Intro")

This is a list of awesome articles about object detection from video.

***

## Datasets

### ImageNet VID Challenge
- **Site**: http://image-net.org/challenges/LSVRC/2017/#vid
- **Kagge**: https://www.kaggle.com/account/login?returnUrl=%2Fc%2Fimagenet-object-detection-from-video-challenge

### VisDrone Challenge
- **Site**: http://aiskyeye.com/

## Paper list

### 2016

#### Seq-NMS for Video Object Detection
- **Date**: 26 Feb 2016
- **Arxiv**: https://arxiv.org/abs/1602.08465

#### T-CNN: Tubelets with Convolutional Neural Networks for Object Detection from Videos
- **Date**: 9 Apr 2016
- **Arxiv**: https://arxiv.org/abs/1604.02532
- **Performance**: 73.8% mAP on ImageNet VID validation.
- **Code**: https://github.com/myfavouritekk/T-CNN

#### Object Detection from Video Tubelets with Convolutional Neural Networks
- **Date**: 14 Apr 2016
- **Arxiv**: https://arxiv.org/abs/1604.04053
- **Code**: https://github.com/myfavouritekk/vdetlib

#### Deep Feature Flow for Video Recognition
- **Date**: 23 Nov 2016
- **Arxiv**: https://arxiv.org/abs/1611.07715
- **Performance**: 73.0% mAP on ImageNet VID validation at 29 fps on a Titan X GPU.
- **Code**: https://github.com/msracver/Deep-Feature-Flow

### 2017

#### Object Detection in Videos with Tubelet Proposal Networks
- **Date**: 21 Feb 2017
- **Arxiv**: https://arxiv.org/abs/1702.06355

#### Flow-Guided Feature Aggregation for Video Object Detection
- **Date**: 29 Mar 2017
- **Arxiv**: https://arxiv.org/abs/1703.10025
- **Performance**: 76.3% mAP at 1.4 fps or 78.4% (combined with Seq-NMS) at 1.1 fps on ImageNet VID validation on a Titan X GPU.
- **Code**: https://github.com/msracver/Flow-Guided-Feature-Aggregation

#### Detect to Track and Track to Detect
- **Date**: 11 Oct 2017
- **Arxiv**: https://arxiv.org/abs/1710.03958
- **Performance**: 79.8% mAP on ImageNet VID validation.
- **Code**: https://github.com/feichtenhofer/Detect-Track

#### Towards High Performance Video Object Detection
- **Date**: 30 Nov 2017
- **Arxiv**: https://arxiv.org/abs/1711.11577
- **Performance**: 78.6% mAP on ImageNet VID validation at 13 fps on a Titan X GPU.

### 2018

#### Object Detection in Videos by High Quality Object Linking
- **Date**: 30 Jan 2018
- **Arxiv**: https://arxiv.org/abs/1801.09823

#### Towards High Performance Video Object Detection for Mobiles 
- **Date**: 16 Apr 2018
- **Arxiv**: https://arxiv.org/abs/1804.05830
- **Performance**: 60.2% mAP on ImageNet VID validation at 25.6 fps on mobiles.

#### Optimizing Video Object Detection via a Scale-Time Lattice
- **Date**: 16 Apr 2018
- **Arxiv**: https://arxiv.org/abs/1804.05472
- **Performance**: 79.4% mAP at 20 fps or 79.0% at 62 fps on ImageNet VID validation on a Titan X GPU.
- **Code**: https://github.com/hellock/scale-time-lattice

#### Object Detection in Video with Spatiotemporal Sampling Networks
- **Date**: 15 Mar 2018
- **Arxiv**: https://arxiv.org/abs/1803.05549
- **Performance**: 80.4% mAP on ImageNet VID validation.

### comparison table

| Paper | Date | Base detector | Backbone | Optical flow? | Online? | mAP(%) | FPS (Titan X) | FPS (on mobiles) |
| ---|---| ---|---|---|---|---|---|---|
| Seq-NMS | 26 Feb 2016 | R-FCN | ResNet101 | no | no | 76.8 | 2.3 | - |
| T-CNN | 9 Apr 2016 | DeepIDNet+CRAFT | - | no | no | 73.8 | - | - |
| DFF | 23 Nov 2016 | R-FCN | ResNet101 | yes | yes | 73.0 | 29 | - |
| FGFA | 29 Mar 2017 | R-FCN | ResNet101 | yes | yes | 76.3 | 1.4 | - |
| FGFA + Seq-NMS | 29 Mar 2017 | R-FCN | ResNet101 | yes | no | 78.4 | 1.14 | - |
| D&T | 11 Oct 2017 | R-FCN (15 anchors) | ResNet101 | no | no | 79.8 | 7.09 | - |
| Scale-time-lattice | 16 Apr 2018 | Faster RCNN (15 anchors)| ResNet101 | no | no | 79.6 | 20 | - |
| Scale-time-lattice | 16 Apr 2018 | Faster RCNN (15 anchors)| ResNet101 | no | no | 79.0 | 62 | - |