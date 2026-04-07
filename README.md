This project implements real-time color detection using a webcam with OpenCV in Python.
It detects a specific color (e.g., yellow) in a video stream, applies noise reduction, and draws a bounding box around the detected region.

The project also uses a helper file `get_limits.py` to dynamically generate HSV color ranges for detection.

Technologies Used:

1) Python
2) OpenCV (`cv2`)
3) NumPy
4) PIL (optional, for alternate bbox method)

Project Structure

```
color-detection/
│── color_detection.py   # Main script
│── util.py              # Contains get_limits() function
│── README.md            # Documentation
```

---

## ⚙️ How It Works

1. Capture Video: The webcam feed is accessed using:
2. Convert to HSV: The frame is converted from BGR to HSV,HSV is preferred because it separates **color (Hue)** from lighting.
3. Get Color Limits: The function `get_limits(color)` returns Lower HSV bound and Upper HSV bound
4. Create Mask: This highlights only the selected color.
5. Noise Removal: with the help of median blur technique to remove unwanted noise.



 `get_limits.py`file :  This file defines how HSV ranges are calculated. To convert a BGR color into an HSV range for detection.

Developed as part of a computer vision learning project 










