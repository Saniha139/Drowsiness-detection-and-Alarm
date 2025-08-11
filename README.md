# Drowsiness Detection System with Alarm Alert
This project is a real-time drowsiness detection system for drivers using deep learning and computer vision. It uses a YOLOv5 object detection model trained to identify whether a person is drowsy or awake from webcam footage. If the system detects drowsiness for more than 10 continuous seconds, it triggers an alarm to alert the driver. The alarm stops once the driver is awake for at least 5 seconds.
This solution aims to prevent accidents caused by driver fatigue, especially on highways or during night-time driving.

---

## Features

- Real-time object detection via webcam
- Fast inference using PyTorch and YOLOv5
- Supports custom-trained YOLOv5 weights
- Simple and lightweight Python implementation

---

## Technologies Used

- Python
- OpenCV
- PyTorch
- YOLOv5 (via `torch.hub`)

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Drowsiness-detection-and-Alarm.git
cd Drowsiness-detection-and-Alarm

```
### 2. Install Dependencies

Install the required dependencies by running:

```bash
pip install -r requirements.txt
```
### 3. Download or Place the YOLOv5 Model Weights
Place your trained model file (last.pt) in the appropriate directory and update the path in the code if needed:

```python
model = torch.hub.load('ultralytics/yolov5', 'custom', path='your/path/to/last.pt')
```
## You can train your own model using the official YOLOv5 repository.

### 4.Run the Script
You can run the code from a .py file or Jupyter Notebook:

```python
python filename.py
```

### Author
Saniha Manjunath
GitHub: @saniha139



