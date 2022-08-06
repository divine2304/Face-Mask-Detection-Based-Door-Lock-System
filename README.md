# Project Title: 
Face Mask Detection Based Door Lock System.
Forked from Tamanna Nazmin's Repository for reference


# Project Description: 
For building face mask based door system, We used machine learning model using Keras, Tensorflow library in python language. After building model we used OpenCV to detect whether a person is wearing a mask or not in real time. This system contains mainly three devices. They are: servo, camera and Arduino Uno. We used arduino Uno to control servo and camera. If someone appears in front of the entrance wearing a mask properly, covering both their mouth and nose, then they will be let in. But if someone appears without a mask then they will be denied entry. This versatile system could be used with variety of entrances with different locking system. the image of demo working project is given below:

# How to run the project

***Step 1***
You have to run 'train_mask_detector.py' file in spyder or Jupyter Notebook to create a model named 'mask_detector.model' using spyder or Jupyter notebook.
For training 'train_mask_detector.py' file you need a dataset having two folders: 
1. withMask
2. Withoutmask. 

***Step 2***
You have to run ‘myDetect.py’ file in spyder. For running this file you need 'res10_300x300_ssd_iter_140000.caffemodel',  'deploy.prototxt' and 'mask_detector.model' file. 
You must connect your webcam with your PC but if you are using Laptop then you don't need any webcam.If you run everything successfully then your camera will be opened and you can test if it works with the mask or not.

***Step 3***
Finally, you will add Serial Command to the facemask detection algorithm that will order the Arduino to send commands to the servo motor.
If you want to use Arduino then first, you have to run and compile 'msdCode.ino' file on the Arduino board using Arduino Software. Next, you have to connect your Arduino with your pc or laptop using a USB cable and then you have to comment out the Arduino code from  'myDetect.py' file and run the file. 

Remember you have to connect your Arduino, servo on a respective port before running the code. 
the connection is given below:


#### For Servo 
###### You have to connect the servo with Arduino digital pin 6
######Connect servo ground with Arduino digital pin ground
######Connect servo power pin with Arduino digital pin 5v


# Language: 
Python and Arduino.
# Library:
tensorflow, keras, imutils, cv2, numpy, time, os, serial
# Hardware:
Arduino Uno, servo, webcam.
# IDE: 
Spyder, Arduino Software, Pycharm
