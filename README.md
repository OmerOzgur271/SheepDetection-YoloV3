# Yolo v3 Object Detection with Tensorflow 1.X
Yolo v3 is an algorithm that uses deep convolutional neural networks to detect objects. <br> <br>

## Getting started

### Prerequisites
This project is written in Python 3.6 using Tensorflow 1.X (deep learning), NumPy (numerical computing), Pillow (image processing), OpenCV (computer vision) and seaborn (visualization) packages.

```
pip install -r requirements.txt
```


## Running the model
You can run the model using `detect.py` script. The script works on images, video or your webcam. Don't forget to set the IoU (Intersection over Union) and confidence thresholds.
### Usage
```
python detect.py <images/video/webcam> <iou threshold> <confidence threshold> <filenames>
```
### Images example
Let's run an example using sample images.
```
python detect.py images 0.5 0.5 data/images/testkoyun.jpeg
```
Then you can find the detections in the `detections` folder.
<br>
You should see something like this.
```
detection_1.jpg
```
![alt text](https://github.com/OmerOzgur271/SheepDetection-YoloV3/blob/main/detections/detection_1.jpg)
```

### Video example
You can also run the script with video files.
```
python detect.py video 0.5 0.5 data/video/koyun.mp4
```
The detections will be saved as 'detections.mp4' in the data/detections folder.
```


