# Invisible-Keyboard
This project implements a hand-tracking-based virtual keyboard using OpenCV, MediaPipe, and Python. The program captures live video from the webcam and detects hand movements to simulate keypresses on a virtual keyboard.
# Features
Real-time hand tracking using MediaPipe.
A virtual keyboard displayed on the screen.
Keypress simulation when the user’s hand hovers over the virtual keys.
Visual feedback for detected keypresses.
# Technologies Used
Python: The main programming language used in this project.
OpenCV: For handling image processing and capturing video from the webcam.
MediaPipe: For hand tracking and gesture detection.
Pynput: To simulate keyboard presses in real-time.
# How it Works
Hand Detection: The program uses MediaPipe to detect hands and track landmarks on the hand.
Key Detection: The position of the index finger (landmark 8) and middle finger (landmark 12) are used to detect interactions with the virtual keyboard.
Virtual Keyboard: A virtual keyboard is drawn on the screen using OpenCV. Each key is represented as a button that reacts when the hand interacts with it.
Key Press Simulation: When the distance between the index and middle fingers is small enough (within a threshold), a simulated keypress is sent using Pynput.
