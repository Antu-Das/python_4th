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
Used roboflow to annotate images. Sample notebook show how we can add the Roboflow workflow project using API to download the annotated dataset to train the model. Use the below code to download the datset:

[(pip install roboflow

from roboflow import Roboflow
rf = Roboflow(api_key="ZxxNYh8DK5KRIhp90MPb")
project = rf.workspace("rehman-2vlay").project("fire-detection-vdtmc")
version = project.version(1)
dataset = version.download("yolov5")]((pip install roboflow

from roboflow import Roboflow
rf = Roboflow(api_key="ZxxNYh8DK5KRIhp90MPb")
project = rf.workspace("rehman-2vlay").project("fire-detection-vdtmc")
version = project.version(1)
dataset = version.download("yolov5"))



## Evaluation

![The below chart show the loss , mAP (mean Average Precision) score for the train, test,validation set.](https://github.com/Antu-Das/python_4th/blob/main/download%20(8).png)

## Confusion Matrix
![Confusion Matrix](https://github.com/Antu-Das/python_4th/blob/main/download%20(3).png)






