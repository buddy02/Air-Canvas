# Aircanvas using OpenCV
This Python script demonstrates a simple real-time drawing application using OpenCV (Open Source Computer Vision Library). 

## Requirements and Installation

- Python 3.x
- OpenCV (cv2)
- NumPy

You can install OpenCV and NumPy using pip:

```bash
  pip install opencv-python numpy
```

## Demo

![aircanvas](https://github.com/buddy02/Air-Canvas/assets/93868306/04ef090f-3839-4a78-a360-b8930903c7c4)

## Run Locally

Clone the project

```bash
  git clone https://github.com/buddy02/Air-Canvas/tree/main
```

After installing the required packages go to the project directory

```bash
  cd Air-Canvas
```

Run the python script

```bash
  python3 aircanvas.py
```
   
## How It Works

Air Canvas employs color detection techniques to track hand movements and enable interactive painting. Here's how color detection works in this project:

- The application captures video frames from your webcam in real-time.
- It converts each frame to the HSV (Hue, Saturation, Value) color space, which is more suitable for color detection than the traditional RGB color space.
- Using adjustable trackbars, you can specify the upper and lower HSV values for different colors, such as blue, green, red, and yellow.
- The application creates a binary mask by thresholding the frame based on the specified HSV color ranges.
- It performs morphological operations like erosion and dilation to clean the mask.
- The project identifies the user's hand based on the mask and extracts its position.
- Hand gestures are recognized, allowing you to draw in different colors or clear the canvas. 
