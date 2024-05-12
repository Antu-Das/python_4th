# python_4th
# Fire Detection using OpenCV for Real Time and Custom Data

## Overview
This project utilizes YOLOv8, a state-of-the-art object detection algorithm, for detecting fires in images and videos. Additionally, it implements an alarm system to alert users in real-time upon detection of a fire.

## Requirements
- Python 3.x
- Pycharm
- OpenCV
- YOLOv8 pre-trained weights
- [Insert any other dependencies here]

## Installation
1. Clone this repository:
   git clone : https://github.com/Antu-Das/python_4th.git
   cd python_4th
2. Install dependencies: pip install -r requirements.txt
3. Download YOLOv8 pre-trained weights 

## Custom Data
Used roboflow to annotate images. Sample notebook show how we can add the Roboflow workflow project using API to download the annotated dataset to train the model. Which roboflow code include in the dataset folder.


## Evaluation

![The below chart show the loss , mAP (mean Average Precision) score for the train, test,validation set.](https://github.com/Antu-Das/python_4th/blob/main/download%20(8).png)

## Confusion Matrix
![Confusion Matrix](https://github.com/Antu-Das/python_4th/blob/main/download%20(3).png)

## Inference
Run the model using below command:

!python train.py model=yolov8s.pt data={dataset.location}/data.yaml epochs=8 imgsz=640

The source argument is required to specify the path to the input video. the above command save your weight in run/predict, which will contain the annotated frames with fire detections.

## Result

![](https://github.com/Antu-Das/python_4th/blob/main/download%20(5).jpeg)

The project can detect fire in real-time  with high accuracy. The detection and tracking performance can be improved by fine-tuning the YOLOv8 model on a custom dataset. It can be used as a starting point for more advanced projects and can be easily integrated into a larger system for fire monitoring.

## Fire detected with alarm

![Watch the video](https://github.com/Antu-Das/python_4th/blob/main/video_2024-05-13_02-31-20.mp4)









