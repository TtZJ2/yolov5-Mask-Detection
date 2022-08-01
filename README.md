# Yolov5: mask detection

```bash
pip install -r requirements.txt

python train.py --data mask_data.yaml --cfg mask.yaml --batch-size 32

python detect.py --weights ./runs/train/exp/weights/best.pt --source data/images --conf 0.25

python test.py --data mask_data.yaml --weights ./runs/train/exp/weights/best.pt
```