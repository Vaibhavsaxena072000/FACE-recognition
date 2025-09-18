# Face Recognition
1)Save the script as face_recog.py in E:/my python/.

2)Put your image file there too: E:/my python/vaibhav down.jpg.
 
3)Open VS Code → select the right Python interpreter (bottom-right).

4)Install dependencies in VS Code terminal:
 pip install opencv-python deepface tensorflow==2.15.0

5)Press Ctrl+F5 (Run Without Debugging).

6)A window should open showing your webcam feed with "MATCH" / "NO MATCH".

7)Press Q to close.

# Librarires used 

1. threading (Python standard library)

Used to run the check_face function in a separate thread, so face verification doesn’t block the video feed.

Helps keep the webcam video smooth while DeepFace processes frames.

2. cv2 (OpenCV)

Handles video capture from the webcam.

Provides image processing functions (cv2.putText, cv2.imshow, cv2.VideoCapture).

Draws "MATCH" / "NO MATCH" text on the video frame.

3. deepface

Main library for facial recognition, verification, and analysis.

DeepFace.verify() compares the live webcam frame with your reference image.

Under the hood, it can use multiple face detectors (like RetinaFace, OpenCV, Dlib, MTCNN).

4. tensorflow / tf-keras

DeepFace depends on TensorFlow to run its deep learning models.

