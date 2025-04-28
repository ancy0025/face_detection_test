# Real-Time Face Detection using OpenCV

This project demonstrates real-time face detection using OpenCV and Haar cascades. The application uses your webcam to detect faces in real-time and draws rectangles around the detected faces.

## Requirements
To run this project, ensure you have the following installed:
- Python 3.x
- OpenCV (`cv2`)

You can install OpenCV using pip:
```bash
pip install opencv-python

How It Works
Load Haar Cascade Classifier: The face detection model used in this code is based on a pre-trained Haar cascade classifier, which is used to detect faces in images.

Start Webcam: The code starts the webcam (cv2.VideoCapture(0)) and captures frames in real-time.

Grayscale Conversion: Each frame is converted to grayscale to improve the performance of face detection.

Detect Faces: The detectMultiScale() function is used to detect faces in the grayscale frame.

Draw Rectangles: For each detected face, a green rectangle is drawn around it.

Display the Frame: The processed frame with rectangles around detected faces is displayed in a window.

Exit Condition: Press the 'q' key to stop the webcam and close the window.

Running the Application
Clone or download the project.

Make sure you have OpenCV installed.

Run the Python script.
