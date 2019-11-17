# Mini-project
# Multi Face Recogniton using Python & OpenCV

OpenCV based face recognition system that can detect and recognize multiple faces in an image.



There are 3 parts in a face recognition system.
 1. Creating datasets (face_datasets.py)
2. Train the model (training.py)
3. Face Recognition (face_recognition.py)

  
# Face Detection.
Face detection is acheived in this project using Haar Cascade classifier. It could be used for object detection. Here we are using it for detecting faces.

# Face Recognition
We are using LBPH (Local Binary Patterns Histograms ) classifier to recognize the faces from the images. It compares neighboring pixels of a pixel and creates a histogram out of it for comparing faces.

Local Binary Patterns Histograms (LBPH) Face Recognizer - `cv2.face.createLBPHFaceRecognizer()`

# Requirements
1. [Python 3.7](https://www.python.org/downloads/)
2. [OpenCV 2](https://opencv.org/releases/)
3. [Numpy](https://www.numpy.org/)

## How to run?

1. Run in the command line the face_datasets.py for taking your face image as datasets.
5. If you have more face to be include, change the ID and run the program again
6. Train your datasets by running training.py
7. Lastly, run face_recognition.py


