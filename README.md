# automatic-number-plate-recognition-python-yolov8

<p align="center">
<a href="https://www.youtube.com/watch?v=fyJB1t0o0ms">
    <img width="600" src="https://utils-computervisiondeveloper.s3.amazonaws.com/thumbnails/with_play_button/anpr_yolo2.jpg" alt="Watch the video">
    </br>Watch on YouTube: Automatic number plate recognition with Python, Yolov8 and EasyOCR !
</a>
</p>

## data

The video I used in this tutorial can be downloaded [here](https://drive.google.com/file/d/1YmHTElM6rh5uBpvaoUYpYTHK2odJkoM6/view?usp=drive_link).

## models

A Yolov8 pretrained model was used to detect vehicles.

A licensed plate detector was used to detect license plates. The model was trained with Yolov8 using [this dataset](https://universe.roboflow.com/roboflow-universe-projects/license-plate-recognition-rxg4e/dataset/4) and following this [step by step tutorial on how to train an object detector with Yolov8 on your custom data](https://github.com/computervisioneng/train-yolov8-custom-dataset-step-by-step-guide). The model is available [here](https://drive.google.com/file/d/1ZKRejyvMO1870mSWH6MZu0lv28xWpSuz/view?usp=drive_link).

## dependencies

The sort module needs to be downloaded from [this repository](https://github.com/abewley/sort) as mentioned in the [video](https://youtu.be/fyJB1t0o0ms?t=1120).

## How to Initialize

* Install required dependencies.
  - pip install -r requirements.txt
* Make sure to downgrade pillow to v 9.5.0
  - pip uninstall Pillow
  - pip install Pillow==9.5.0
* Clone the following repository in to the root folder (make sure the cloned folder is renamed to 'sort').
  - git clone https://github.com/abewley/sort.git
* Create following folders in the root folder.
  - models
  - input
  - output
  - csv
* Download [yolov8n.pt](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) & [license_plate_detector.pt](https://drive.google.com/file/d/1ZKRejyvMO1870mSWH6MZu0lv28xWpSuz/view) and move them to the 'models' folder.
* Rename the input video as 'sample' and move it to the 'input' folder.

## How to Run

* Run main.py (this may take some time)
* Run add_missing_data.py
* Run visualize.py

  You can find the output video in the 'output' folder !
