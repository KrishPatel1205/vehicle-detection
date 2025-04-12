# Vehicle Detection using YOLO 🚗🚌🚑🏍️🚛

A computer vision project built with [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) to detect and classify vehicles in real-time using either a webcam or a video file as input. The model detects and classifies vehicles into five categories: `Ambulance`, `Bus`, `Car`, `Motorcycle`, and `Truck`.

## 🔍 Features

- 📹 Real-time detection via webcam or video file
- 🎯 Custom-trained YOLO model with 5 vehicle classes
- 📦 Bounding boxes with labels drawn on detected vehicles
- 📁 Outputs are saved with annotated video frames
- 🛠️ CLI interface for flexible usage

## 🚀 Classes Used

| ID | Class Name   |
|----|--------------|
| 0  | Ambulance    |
| 1  | Bus          |
| 2  | Car          |
| 3  | Motorcycle   |
| 4  | Truck        |

## 🖥️ Demo

![demo gif or image here, optional]

## 🧰 Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/vehicle-detection.git
cd vehicle-detection
```

2. **Run using command line**

```bash
python3 yolo_detect.py --model my_model.pt --source <Destination to your video file> --resolution 1920x1080
```

alternatively run using your camera with 

```bash
python3 yolo_detect.py --model my_model.pt --source usb0 --resolution 1920x1080
```
