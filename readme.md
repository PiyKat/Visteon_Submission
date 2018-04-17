# VISTEON TASK SUBMISSION

The repository contains the work done for the task given to me by the respected authority.

# SOLUTION

There are essentially two important steps that need to be taken to complete the task -

1. Robust vehicle detection algorithm - For this purpose, I have used two approaches. The first one is a traditional CV aaproach where I have trained a Haar Cascade and the second approach leverages deep learning techniques and the approach is popularly known as You Only Look Once(YOLO) approach.

2. Detection of abrupt stopping of the vehicle - For this task, we can use two approaches. The first one involves object flow, and the second one involves putting threshhold on bounding box size change.


# VEHICLE DETECTION

## Haar Classifier

In this approach, I used the [Stanford Cars Dataset](https://ai.stanford.edu/~jkrause/cars/car_dataset.html) for the positive samples and [MIT Vision Texture Dataset](http://vismod.media.mit.edu/vismod/imagery/VisionTexture/vistex.html) for negative samples. Due to the time constraint, I trained it on a very small subset of the aforementioned datasets.

To run this approach, just run the car_detection.py file in the folder.

## YOLO Object Detector

The YOLO Approach was created using Tensorflow 0.12.1 version. The model's size was ~350MB, thus I didn't upload it directly, but you can download it from [this page](https://drive.google.com/file/d/0B5WIzrIVeL0WS3N2VklTVmstelE/view). 


# STOP SIGN INDICATOR

For this task, the approach was to first implement object flow on the detected vehicles and check if there is an abrupt change in the flow. In conjunction, we would also measure the rate of change of the size of the bounding box and if it exceeds a threshold value, we can display a stop sign. Due to some technical issues and the deadline, this could not be completed as intended.
