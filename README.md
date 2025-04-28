# Face Detection with OpenCV

A Python script for real-time face detection using OpenCV's Haar Cascade Classifier. It captures webcam video and draws green rectangles around detected faces.

## Prerequisites
- Python 3.x
- OpenCV (`opencv-python`): Install with `pip install opencv-python`
- A connected webcam

## Dependencies
- `cv2` (OpenCV)

## Usage
1. Connect a webcam.
2. Save the script as `face_detection.py`.
3. Run: `python face_detection.py`
4. View the webcam feed with detected faces.
5. Press `q` to quit.

## How It Works
- Loads `haarcascade_frontalface_default.xml` for face detection.
- Captures video from the default webcam (index `0`).
- Converts frames to grayscale and detects faces using `detectMultiScale` (scaleFactor=1.1, minNeighbors=5).
- Draws green rectangles around faces.
- Displays the feed in a window ("Face Detection Test").
- Exits on `q` keypress and releases resources.

## Troubleshooting
- **Webcam not found**: Check connection or try `VideoCapture(1)`.
- **Cascade file error**: Reinstall OpenCV or verify `cv2.data.haarcascades` path.
- **Lag**: Lower resolution or adjust `scaleFactor`/`minNeighbors`.

## License
This project is licensed under the MIT License. 
