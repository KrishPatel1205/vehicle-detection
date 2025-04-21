# 🚗 Vehicle Detection

This project is a real-time vehicle detection system built using [Ultralytics YOLO](https://github.com/ultralytics/ultralytics). It identifies and classifies different types of vehicles in both live webcam feeds and pre-recorded videos.

The model was **custom-trained** on a dataset I created from scratch using real-world traffic footage. I manually labeled thousands of images to build a dataset tailored for detecting five specific vehicle categories: `Ambulance`, `Bus`, `Car`, `Motorcycle`, and `Truck`. This helped the model perform accurately in real-world urban scenarios.


## 🔍 Features

- 📹 Real-time detection via webcam or video file  
- 🎯 Custom-trained YOLO model with 5 vehicle classes  
- 📦 Bounding boxes with labels drawn on detected vehicles  
- 💾 Outputs saved with annotated video frames  
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

### Example 1



https://github.com/user-attachments/assets/18094094-1229-4e02-8b5b-4a81cd6e2cd5



---

### Example 2



https://github.com/user-attachments/assets/6a7f8531-5e98-414b-a64e-d29872e4aa26




## 🧰 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/vehicle-detection.git
cd vehicle-detection
```

### 2. Download YOLO Detection Script

```bash
curl -o yolo_detect.py https://raw.githubusercontent.com/EdjeElectronics/Train-and-Deploy-YOLO-Models/refs/heads/main/yolo_detect.py
```

### 3. Install PyTorch

Visit [pytorch.org](https://pytorch.org/) to install the correct version for your system.

Example for M2 Pro MacBook:

```bash
pip3 install torch torchvision torchaudio
```

## ▶️ Running the Model

### Using a Video File

```bash
python3 yolo_detect.py --model my_model.pt --source <path_to_video_file> --resolution 1920x1080
```

### Using a Webcam

```bash
python3 yolo_detect.py --model my_model.pt --source usb0 --resolution 1920x1080
```
