# 🎯 Color-Based Object Tracking

## Overview
This project allows you to track **red objects** in real-time using your computer's camera.  
It detects the object, draws a rectangle around it, and shows its **center coordinates** and **size** on the screen.  
The program is written using **Python** and **OpenCV**, designed to be simple and beginner-friendly, ideal for a student-level project.

## Features
- Detects red objects in real-time.
- Draws a green rectangle around each detected object.
- Displays the object's **center coordinates** (x, y) and **width x height**.
- Shows a mask view highlighting the detected red areas.
- Simple, clear, and easy to understand code for learning purposes.

## How It Works
1. The camera feed is captured frame by frame.
2. Each frame is converted from BGR to HSV color space for better color detection.
3. A mask is created to detect red color in two HSV ranges.
4. Noise in the mask is removed using morphological operations.
5. Contours of the masked areas are found to locate the objects.
6. For each sufficiently large contour:
   - A rectangle is drawn around the object.
   - The object's center coordinates and size are displayed above the rectangle.
7. Two windows are displayed:
   - **Camera**: shows the live feed with rectangles and coordinates.
   - **Mask**: shows the detected red areas in white on a black background.

## Installation
1. Make sure you have Python 3 installed.
2. Install the required libraries:
```bash
pip install -r requirements.txt

1.Run the program:
python main.py

2.Show a red object in front of your camera.

3.Observe the rectangle, coordinates, and size displayed on the video.

4.Press q to quit the program.

### Files
main.py → Main program that captures camera feed and tracks objects.
requirements.txt → Contains necessary Python packages.
README.md → Project explanation and instructions.

 ### Notes
The program ignores very small red areas to reduce noise.
You can adjust the HSV red ranges in the code if needed.
Works best with well-lit environments.
