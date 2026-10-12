# Warehouse-Object-Detection-using-YOLO



Fine-tuned YOLO11n to detect objects in a warehouse scene (6 classes).

## Dataset
WAREHOUSE Computer Vision Dataset by tawadhu3 (Roboflow Universe), CC BY 4.0.
1,800 images; train/valid/test: 1655/145/none. Classes: Acc, Kain, Kain-Acc-Person, forklif, hand-pallet, person.

## Method
- Model: YOLO11n (Ultralytics), fine-tuned for 30 epochs at 640x640 on a Colab T4
- [Tracking: ByteTrack on video]   <- delete this line if you didn't do it
- [Export: ONNX]                   <- delete this line if you didn't do it

## Results
mAP50: 0.988, mAP50-95: 0.619 on the validation split (145 images).
Note: images are consecutive frames from fixed cameras, so these results are likely optimistic.

## Files
best.pt, results.png, confusion_matrix.png, notebook
