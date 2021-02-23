# Object detection

## This repo briefly presents application of TensorFlow object detection API (tensorflow/models/tree/master/research/object_detection) for tracking and counting human spermatozoa in microscopic video. The project was conducted using a open-access visem dataset (https://datasets.simula.no/visem/)

## Data preparation:
Training and test data was prepared using 50 snapshots from several videos and then manually annotated with https://github.com/tzutalin/labelImg (go to sperm_detection/test/ for examples)

## Model and training:
Training process was performed with transfer learning aproach on model **ssd mobilenet v2** in Google Colab (object_detection.ipynb)

## Detection:
Final stage consisted of running trained **ssd mobilenet v2** with TensorFlow object counting API https://github.com/ahmetozlu/tensorflow_object_counting_api

## Output:
Final results are located under https://drive.google.com/drive/folders/1mlFu8W7NAF9CJlgPxMNseEgGXSEfEo-u?usp=sharing

**room/** contains test run with off-the-shelf **ssd mobilenet v2** and **mask rcnn** trained on COCO (https://cocodataset.org/#home)

**sperm_count** contains final results of the project using **ssd mobilenet v2**



