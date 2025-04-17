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

### Example 1:

**Before:**

https://github.com/user-attachments/assets/0d61d228-75fd-4159-ae85-7a298b14a285



**After:**

https://github.com/user-attachments/assets/40056ad8-b4b8-4edc-b6ea-f364281e747c


### Example 2:

**Before:**


https://github.com/user-attachments/assets/f3eb9aaf-2a6b-4388-89fa-441590caaeb8

**After:**

https://github.com/user-attachments/assets/9e4c934b-5703-4e57-8b13-65de4c09066f


### Example 3:

**Before:**

https://github.com/user-attachments/assets/1ed357f9-3f5e-4306-8181-bb10b65c3f79

**After:**

https://github.com/user-attachments/assets/2a2386ba-a3ac-4f52-8043-67295e816918


## 🧰 Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/vehicle-detection.git
cd vehicle-detection
```

2. **Install Yolo**


```bash
curl -o yolo_detect.py https://raw.githubusercontent.com/EdjeElectronics/Train-and-Deploy-YOLO-Models/refs/heads/main/yolo_detect.py
```

3. **Install PyTorch**
   
   Go to the PyTorch website and install the correct verison for your model
   
   For example: ``` pip3 install torch torchvision torchaudio ``` works for my M2 Pro Macbook Pro

5. **Run using command line**

```bash
python3 yolo_detect.py --model my_model.pt --source <Destination to your video file> --resolution 1920x1080
```

alternatively run using your camera with 

```bash
python3 yolo_detect.py --model my_model.pt --source usb0 --resolution 1920x1080
```
