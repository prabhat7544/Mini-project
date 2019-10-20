# Mini-project
# Multi Face Recogniton using Python & OpenCV

OpenCV based face recognition system that can detect and recognize multiple faces in an image.



There are 2 parts in a face recognition system.
  1. Face Detection - To detect faces in image.
  2. Face Recognition - To recognize face of  persons in the image.
  
# 1. Face Detection.
Face detection is acheived in this project using Haar Cascade classifier. It could be used for object detection. Here we are using it for detecting faces.

# 2. Face Recognition
We are using LBPH (Local Binary Patterns Histograms ) classifier to recognize the faces from the images. It compares neighboring pixels of a pixel and creates a histogram out of it for comparing faces.

Local Binary Patterns Histograms (LBPH) Face Recognizer - `cv2.face.createLBPHFaceRecognizer()`

# Requirements
1. [Python 2.7.x](https://www.python.org/downloads/)
2. [OpenCV 2](https://opencv.org/releases/)
3. [Numpy](https://www.numpy.org/)

## How to run?
To run the program, in terminal type “python face_rec.py”

The photos of each individual should be stored in a folder (s1, s2 etc) inside the training-data folder.
Test images are stored in test-data folder.

The application is built over 3 files. 
  1. face_rec.py - Create the recognizer, train the images using `training_data()` and makes predictions from test data using `predict()` function.
  2. training_data.py - To parse through each images in the training set and call `face_detect()` on each image.
  3. face_detect.py - To detect the face, here we are initializing Haar Cascade classifier to detect multiple faces from the image, draw bounding boxes over face and returns the face bonding box coordinates.

