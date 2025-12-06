# Color-Based Object Tracking – Real-Time Red Detection

> **Domain:** Computer Vision / Image Processing  
> **Level:** Beginner (Student R&D)  
> **Purpose:** Demonstrate color-based object tracking in a real-time camera stream using Python and OpenCV

---

## 1. Background & Concept
Color detection is a common technique in introductory computer vision, providing a clear way to learn frame processing, color space conversions and basic contour operations.  
This project builds a minimal real-time object tracking system focused on detecting red regions and drawing bounding boxes around them.

---

## 2. Features
- Real-time red object detection  
- Bounding box with center coordinates  
- Object dimensions displayed (width × height)  
- Mask visualization window  
- Simple OpenCV-based implementation  
- Beginner-friendly code and structure  

---

## 3. How It Works
1. Capture live video frames from the webcam  
2. Convert each frame from BGR to HSV  
3. Create a binary mask using two HSV red ranges  
4. Apply morphological operations to remove noise  
5. Extract contours from the mask  
6. For sufficiently large regions:
   - draw rectangle
   - show coordinates and size  

Two windows are displayed:
- **Camera** – bounding boxes and coordinates  
- **Mask** – detected red regions

---

## 4. Installation
```bash
pip install -r requirements.txt
