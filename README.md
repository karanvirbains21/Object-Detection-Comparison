# Object-Detection-Comparison
Comparison of Faster RCNN, Mask RCNN, and YOLOv8 computer vision models on a set of images.

# Object Detection Model Comparison

## Overview
This project compares two deep-learning object detectors (YOLOv8 and Faster R-CNN) on a set of images. For each image the code records:
- time (seconds) taken by each model
- detected objects and their probabilities
- number of detections

It also produces annotated images and summary CSVs.

## Files
- `Object Detection Comparison.ipynb` : main script 
- `results.csv` : contains the average metrics
- `summary.csv` : contains detailed information for each image
- `README.md` : this file

## Requirements
- Python 3.9+
- pip packages:
  - torch, torchvision (CPU or CUDA build)
  - ultralytics
  - pillow, pandas, tqdm, opencv-python, pytesseract (optional)

## Usage
1. Put at least 10 images in `images/` (jpg/png).
2. Install requirements.
3. Run (CPU):
   ```bash
   python Object Detection Comparison.ipynb --input_dir images --output_dir output --device cpu
