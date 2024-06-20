Hand Gesture Volume Control

This project uses a webcam, OpenCV, and MediaPipe to control the system volume based on hand gestures. By measuring the distance between the thumb and index finger, the volume is adjusted accordingly.

Requirements

- Python 3.x
- OpenCV
- MediaPipe
- Pycaw
- Numpy
- Comtypes

Installation

.Clone the repository or download the code.


Usage

1. Ensure your webcam is connected and working.


2. Adjust the system volume by moving your thumb and index finger closer or farther apart in front of the webcam.

Code Explanation

The script performs the following steps:

1. Setup:
   - Import necessary libraries.
   - Initialize MediaPipe Hands for hand tracking.
   - Setup Pycaw for volume control.

2. Main Loop:
   - Capture frames from the webcam.
   - Convert the frame to RGB.
   - Process the frame to detect hand landmarks.
   - If hand landmarks are detected, extract the coordinates of the thumb and index finger.
   - Calculate the distance between the thumb and index finger.
   - Interpolate the distance to a volume level.
   - Adjust the system volume using Pycaw.
   - Display the volume level on the screen.

Troubleshooting

- Ensure the webcam is properly connected and recognized by your system.
- If the hand landmarks are not detected, try adjusting the lighting conditions.

Future Improvements

- Add support for more gestures to control different functionalities.
- Improve the accuracy of hand landmark detection in varying lighting conditions.
