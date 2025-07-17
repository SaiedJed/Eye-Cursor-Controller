# Eye-Guided Cursor Control

**Eye-Guided Cursor Control** is a webcam-based assistive technology system designed to help individuals—especially those with motor disabilities—control their computer cursor using only their eye movements. Unlike many existing systems that require expensive hardware such as 3D cameras or infrared sensors, this project runs entirely on a standard webcam and leverages machine learning and deep learning models for accurate face and eye detection.

---

##  Overview

This project was developed to support users with disabilities such as ALS or Locked-In Syndrome, enabling them to interact with computers through eye gestures captured by a webcam. The system includes:

- Real-time **gaze tracking**
- **Blink-based clicking**
- A custom **virtual keyboard**
- **Magnification** support for precise interaction
- **Voice commands** for additional control

---

## Demo

A live demo is available and demonstrates the full functionality of the project.  
👉 **[Demo Link – https://drive.google.com/file/d/1_dbMrfWjTWLyd_oYVxgBC2ov4gN7An2S/view?usp=sharing]**

---

##  Features

- **Webcam-only** solution (no special hardware)
- **Face and Eye Detection** using `RetinaFace` and Haar Cascade
- **Gaze Direction Estimation** using deep learning models such as CNN, AGE-Net, and L2CS
- **Real-time Cursor Movement**
- **Blink to Click** mechanism
- **Calibration** for improved personalization and accuracy
- **Virtual Keyboard** optimized for accessibility
- **Magnification Tool** for enhanced target selection
- **Voice Support** for command triggering

---

##  Models and Datasets

- **Face Detection**: RetinaFace (MobileNet-0.25)
- **Eye Detection & Pupil Centering**: Custom morphological processing
- **Gaze Estimation**: L2CS-based regression
- **Datasets Used**:
  - MPIIGaze
  - MPIIFaceGaze
  - Custom in-house dataset for user-specific calibration

---

## Tech Stack

- Python
- OpenCV
- TensorFlow & PyTorch
- Dlib
- YOLOv5 (experimented)
- Google Colab (for training heavy models)

---

## Calibration and Usage
At startup, the app will walk you through a calibration process.

After calibration, your eyes will control the mouse pointer.

A blink will trigger a click.

The virtual keyboard appears automatically in typing fields.

Use voice commands (if enabled) for optional control.

---

## Performance
Tested on various lighting conditions with custom calibration

Accuracy improves with:

Good lighting

Consistent webcam positioning

User training and model personalization
