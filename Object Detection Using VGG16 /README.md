# 🛩️ Object Detection Using VGG16 With TensorFlow
This project demonstrates how to use the **VGG16 pre-trained model** with **TensorFlow** for object detection. Specifically, it detects **airplanes** in images by training a custom **bounding box regression head** on top of the VGG16 feature extractor.

> 📍 Implemented in Google Colab – Notebook: `Object Detection Using VGG16 With Tensorflow.ipynb`

## 📌 Project Overview
The project focuses on detecting airplanes within images using a supervised learning approach. A custom dataset with bounding box annotations is used to fine-tune a model that predicts the location of airplanes by regressing the bounding box coordinates.

## 🗂️ Dataset
- Contains airplane images along with corresponding **bounding box annotations**.
- Annotation format: CSV file with coordinates (`startX`, `startY`, `endX`, `endY`) for each image.
- The dataset is split into training and testing sets for evaluation.

## 🧠 Model Architecture
- **Base Model**: VGG16 pre-trained on ImageNet
- `include_top=False` to remove classification layers
- Used as a **fixed feature extractor**
- **Custom Head**: Bounding box regression layers
- Fully connected (Dense) layers with ReLU activation
- Final layer outputs 4 values: `[startX, startY, endX, endY]`

## 🏋️ Training
- **Optimizer**: Adam
- **Loss Function**: Mean Squared Error (MSE)
- **Batching**: Data split into mini-batches
- **Epochs**: Model trained over multiple iterations for optimal learning

## 📊 Evaluation
- Evaluated on the test set using **Mean Squared Error (MSE)**
- Performance reflects how accurately the model predicts bounding boxes of airplanes in unseen images

## 🚀 Usage
To use the trained model:
1. Load the saved model file (`.h5` or `.pb`)
2. Preprocess an input image
3. Run prediction → Model returns bounding box coordinates
4. Use OpenCV to draw the predicted bounding box on the image

## 💻 Requirements
Install the following libraries:
```bash
pip install tensorflow keras opencv-python numpy scikit-learn imutils matplotlib

🧠** What I Learned**
- Leveraging pre-trained CNNs like VGG16 for custom tasks
- Designing and training a regression head for object detection
- Handling image annotation data and preparing it for training
- Evaluating model performance for bounding box predictions

🙏 **Acknowledgements**
- VGG16 Model
- TensorFlow and Keras documentation
- OpenCV for visualization
- Dataset preparation inspired by various object detection tutorials

📁 **Project Structure**
Object-Detection-VGG16/
├── Object Detection Using VGG16 With Tensorflow.ipynb
├── README.md
├── dataset/
│   ├── images/
│   └── annotations.csv
├── model/
│   └── vgg16_airplane_detector.h5
└── results/
    └── sample_predictions.png


