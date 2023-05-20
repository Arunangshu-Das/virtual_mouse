# Arunangshu's Virtual Mouse

This project implements a virtual mouse using hand tracking and control with the help of computer vision techniques. The code utilizes the Mediapipe library for hand detection and tracking, OpenCV for video processing, and PyAutoGUI for mouse control.

## Prerequisites

Before running the code, make sure you have the following libraries installed:

- OpenCV (cv2)
- Mediapipe (mp)
- PyAutoGUI
- NumPy (numpy)

You can install these libraries using pip:

```
pip install opencv-python mediapipe pyautogui numpy
```

## Usage

1. Connect a webcam to your computer.
2. Run the code using a Python interpreter.
3. A window named "Arunangshu's Virtual Mouse" will appear, showing the webcam feed and tracking information.
4. Place your hand in front of the webcam, making sure it is well-lit and visible.
5. Move your index finger to control the mouse cursor. The cursor will follow the movement of your index finger.
6. Touch your thumb to your index finger to simulate a mouse click. A click event will be triggered when the distance between your thumb and index finger is within a certain threshold.

## Notes

- The code assumes that the webcam is connected as the primary video input device (change `cap=cv2.VideoCapture(1)` to `cap=cv2.VideoCapture(0)` if your webcam is the default device).
- The virtual mouse control is limited to the screen size, so ensure that your screen resolution is properly configured.
- Adjust the threshold value (`20` in the code) for the thumb and index finger distance according to your preference and hand size.
- Press the 'q' key to quit the program and close the window.

## Demo
[**Demo Project Link**](https://youtu.be/9dseVeZsafE)

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The hand tracking and detection functionality is implemented using the Mediapipe library.
- The mouse control is achieved using the PyAutoGUI library.
- Thanks to the OpenCV community for providing the computer vision capabilities used in this project.
