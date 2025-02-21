# Parking Space Detection

Dataset source: http://cnrpark.it/

There are two main parts of the project.

## 1. Parking Car Detection

I used YOLO(v11n) model to detect cars in parking and Roboflow for data annotation and then export it in YOLO format to use it in model training.

## 2. Parking Lot Segmentation

I used UNET to train the model for parking lot segmentation. From  Roboflow, I annotate data and then export it in COCO JSON format. I created mask image using the coco json file, and images and mask images are used to train the UNET model.