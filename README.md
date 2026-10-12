# Warehouse-Object-Detection-using-YOLO



Fine-tuned YOLO11n to detect objects in a warehouse scene (6 classes).

## Dataset
WAREHOUSE Computer Vision Dataset by tawadhu3 (Roboflow Universe), CC BY 4.0.
1,800 images; train/valid/test: 1655/145/none. Classes: Acc, Kain, Kain-Acc-Person, forklif, hand-pallet, person.

## Method
- Model: YOLO11n (Ultralytics), fine-tuned for 30 epochs at 640x640 on a Colab T4
- [Tracking: ByteTrack on video]   
- [Export: ONNX]                   

## Results
mAP50: 0.977, mAP50-95: 0.622 on the validation split (145 images), using best.pt.
Note: images are consecutive frames from fixed cameras, so these results are likely optimistic.
Per-class results are uneven: forklift has 24 validation instances and hand-pallet only 5, so those numbers are weak evidence. Kain-Acc-Person has no validation instances.

## Files
best.pt, results.png, confusion_matrix.png, notebook
