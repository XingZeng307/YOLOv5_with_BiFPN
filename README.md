# YOLOv5_with_BiFPN

YOLOv5 implementation is completely from the original repository (https://github.com/ultralytics/yolov5). 
This repo is mainly for replacing PANet with BiFPN in YOLOv5, which you can check in models/yolov5x.yaml. I didn't use the exact same BiFPN in the paper, while I try to be consistent with yolov5, so still three scale predictions.

# Training

python train.py --img 640 --batch 8 --epochs 200 --data CUB.yaml --weights '' --cfg yolov5x.yaml

I didn't use pre-trained weights since the architecture changes a bit. And as for the performance, I will check more dataset and update it.
