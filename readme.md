# Real-time Detection of Birds for Farm Surveillance Using YOLOv7 and SAHI

There are various causes of crop damage, and a flock of birds serves a major proportion of it. The conventional manual scaring techniques have proven to be inefficient. But the main problem is early detection of birds in the sky, where the acoustic methods prove to be less accurate. Here, the computer vision techniques come to the picture. In this study we train YOLOv7 (You Only Look Once) models and use it in co-ordination with SAHI (Slicing Aided Hyper Inference). We detect a flock of birds by counting the number of bounding boxes of birds detected in a frame of the live video feed captured through cameras, if that number is found to be greater than the decided threshold, an alarm/actuator is turned on to scare away the birds. We train two models, one for RGB videos for day-time monitoring and one for infrared videos for night-time monitoring. Finally, to test our model for accuracy and real-time performance we compute the f1 score, precision, recall and average frames per second. These types of models can be used for farm surveillance, wild animals’ detection, wind farm monitoring, endangered species counting and monitoring the vicinities of an aircraft. We observed that in case of IR Model the number of detections increased by 82% and in case of RGB Model the number of detections increased by 136.6% when SAHI was used on top of YOLOv7.

This repository is based on [YOLOv7](https://github.com/WongKinYiu/yolov7) and [SAHI](https://github.com/obss/sahi).
 

# Paper Citation
```
@INPROCEEDINGS{10273929,
  author={Chaurasia, Divyansh and Patro, B.D.K.},
  booktitle={2023 3rd International Conference on Computing and Information Technology (ICCIT)}, 
  title={Real-time Detection of Birds for Farm Surveillance Using YOLOv7 and SAHI}, 
  year={2023},
  volume={},
  number={},
  pages={442-450},
  keywords={Computer vision;Computational modeling;Biological system modeling;Atmospheric modeling;Surveillance;Transfer learning;Wind farms;REALTIME DETECTION;SURVEILLANCE;COMPUTER VISION;DEEP LEARNING;YOLOv7;SAHI},
  doi={10.1109/ICCIT58132.2023.10273929}}

```

# Dataset used 
```
1.   https://universe.roboflow.com/object-detection/ detection-sbbq4
2.   https://universe.roboflow.com/object-detection/ det1-cvt2f
```

#Getting Started


```
1. Train the YOLOv7 Model. (You can follow the video - https://www.youtube.com/watch?v=5nsmXLyDaU4 for easier understanding).
2. Perform the inference with SAHI. (The code is in yolov7_SAHI).
```

