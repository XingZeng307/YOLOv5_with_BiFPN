# YOLOv5_with_BiFPN

YOLOv5 implementation is completely from the original repository (https://github.com/ultralytics/yolov5). 
This repo is mainly for replacing PANet with BiFPN in YOLOv5, which you can check in models/yolov5x.yaml. I didn't use the exact same BiFPN in the paper, while I try to be consistent with yolov5, so still three scale predictions.

# Training

python train.py --img 640 --batch 8 --epochs 200 --data CUB.yaml --weights '' --cfg yolov5x.yaml

I didn't use pre-trained weights since the architecture changes a bit. And as for the performance, I will check more dataset and update it.


# Reference

https://github.com/ultralytics/yolov5

https://github.com/zylo117/Yet-Another-EfficientDet-Pytorch/tree/15403b5371a64defb2a7c74e162c6e880a7f462c

Mingxing Tan, Ruoming Pang, and Quoc V Le. EfficientDet: Scalable and efficient object detection. In Proceedings
of the IEEE Conference on Computer Vision and Pattern
Recognition (CVPR), 2020.
