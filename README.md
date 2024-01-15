# yolov5_obb
This repository is forked from [yolov5_obb](https://github.com/hukaixuan19970627), which is a custom model of YOLOv5 using oriented bounding boxes.

To use the model in my environment below, I encountered several issues.

After troubleshooting, I documented the issues and modifications of codes on the Wiki.

## Environment

- Windows 10
- Python 3.10
- cuda toolkit 11.8 (11.3+ required)
- cuda driver 12.2
- GeForce RTX 3060

## Modification
There is a new parameter `return_result` on detect.py, returning array of *(class, [x1,y1,x2,y2,x3,y3,x4,y4], conf)*.

## Model Training
If you have trouble training a model with the original repository, you can use my [train_model.ipynb](https://github.com/Jinops/conveyor-alignment-robot/blob/main/model/train_model.ipynb).

## Server
https://github.com/Jinops/conveyor-alignment-robot/blob/main/server/server.py

## Wiki
https://github.com/Jinops/yolov5_obb/wiki/Troubleshooting
