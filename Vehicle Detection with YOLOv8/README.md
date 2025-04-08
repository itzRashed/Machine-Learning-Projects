# 🚗 Vehicle Detection with YOLOv8
This project utilizes the **YOLOv8** object detection model to detect **vehicles** in images and videos. It includes steps for data preparation, model training, and inference, developed using **Python** and **Ultralytics YOLOv8**.

## 🎯 Overview
The objective is to build a powerful vehicle detection model using YOLOv8. The project demonstrates end-to-end object detection workflows from dataset preparation to real-time inference on images and videos.

## 📁 Project Structure
vehicle-detection-yolov8/ 
├── data/ # Vehicle dataset (images and labels)
├── training_results/ # YOLOv8 training outputs and weights 
├── test_images/ # Sample images for inference 
├── videos/ # Sample videos for inference 
├── output/ # Inference results 
└── README.md # Project documentation

## 📦 Requirements
- Python ≥ 3.7  
- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)  
- Google Colab (optional)  
- Libraries: `tqdm`, `shutil`, `os`, `random`, `opencv-python`, `matplotlib`, `torch`, `numpy`

## ⚙️ Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/vehicle-detection-yolov8.git
cd vehicle-detection-yolov8

# Install dependencies
pip install -r requirements.txt

🗂️ Data Preparation
1. Download and organize your dataset like this:
data/
├── train/
│   ├── images/
│   └── labels/
└── valid/
    ├── images/
    └── labels/
2. Use the train_test_split() method if needed to split your dataset.

🧠 Model Training
Update your dataset.yaml with correct paths for training and validation sets.
Train your YOLOv8 model:
bash
yolo task=detect mode=train model=yolov8s.pt data=dataset.yaml epochs=10 imgsz=640 batch=8 project=training_results name=vehicle
Customize training parameters such as epochs, imgsz, or batch as per your needs.

🔍 Inference
🔹 Image Inference
bash
yolo task=detect mode=predict model=training_results/vehicle/weights/best.pt conf=0.55 source=test_images

🔹 Video Inference
bash
yolo task=detect mode=predict model=training_results/vehicle/weights/best.pt conf=0.77 source=videos
➡️ Inference results are saved in runs/detect/.

💡 Notes
- Project is optimized for Google Colab, but can be easily adapted for local use.
- Always double-check your file paths before training and testing.

🧠 What I Learned
- Hands-on implementation of YOLOv8
- Object detection workflow using a custom dataset
- Visualization and performance tuning of models
- Real-time video analysis using deep learning

🙌 Acknowledgements
- Ultralytics YOLOv8
- Open-source vehicle datasets
- Colab and PyTorch communities
