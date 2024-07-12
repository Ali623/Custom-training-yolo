# Custom-training-yolov7

This guide provides instructions on how to run YOLOv7 using pretrained weights. Follow the steps below to get started.

## Prerequisites

Ensure you have the following installed on your system:
- Python 3.7 or higher
- Git
- pip (Python package installer)

## Steps to Run YOLOv7

### 1. Clone the YOLOv7 Repository

First, clone the YOLOv7 repository from GitHub:

```bash
git clone https://github.com/WongKinYiu/yolov7.git
cd yolov7
```

## Install Dependencies
Navigate to the cloned repository and install the required dependencies:

```bash
pip install -r requirements.txt
```

## Download Pretrained Weights
Download the pretrained weights for YOLOv7. You can find the pretrained weights here. For example, download yolov7.pt:

```bash
wget https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt
```


## Run Inference
You can now run inference using the pretrained weights. Replace YOUR_IMAGE.jpg with the path to your image file:

```bash
python detect.py --weights yolov7.pt --source YOUR_IMAGE.jpg
```

This command will use the pretrained weights to detect objects in the specified image.

## Output
The output image with detected objects will be saved in the runs/detect/exp directory. You can view the results by navigating to that directory:

```bash
ls runs/detect/exp
```