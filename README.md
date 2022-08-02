# Mask Detection
## YOLOV5: https://github.com/ultralytics/yolov5
## Classes of number：2
['n','y']  or  ['no-mask','masked']

## Requirements
Python 3.8 or later with all [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) dependencies installed, including `torch>=1.7`. To install run:
```bash
pip install -r requirements.txt
```
## Training
```bash
python train.py --data mask_data.yaml --cfg mask.yaml --batch-size 32
```
## Detecting and Testing
```bash
python detect.py --weights ./runs/train/exp/weights/best.pt --source data/images --conf 0.25

python test.py --data mask_data.yaml --weights ./runs/train/exp/weights/best.pt
```
## Results
<img src="https://github.com/TtZJ2/yolov5-Mask-Detection/blob/main/runs/detect/4.jpg" width="900">
<img src="https://github.com/TtZJ2/yolov5-Mask-Detection/blob/main/runs/detect/a.jpg" width="900">
<img src="https://github.com/TtZJ2/yolov5-Mask-Detection/blob/main/runs/detect/OIP-C.jpg" width="900">
<img src="https://github.com/TtZJ2/yolov5-Mask-Detection/blob/main/runs/detect/4_Dancing_Dancing_4_490.jpg" width="900">

