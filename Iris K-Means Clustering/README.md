# 🌸 Iris K-Means Clustering
This project demonstrates the application of the **K-Means clustering algorithm** on the classic **Iris dataset**, which contains measurements of sepal length, sepal width, petal length, and petal width for 150 iris flowers belonging to three species.

## 🎯 Overview
The goal of this project is to explore unsupervised learning using **K-Means clustering** and visualize how the algorithm groups similar data points in the Iris dataset. We also use the **Elbow method** to determine the optimal number of clusters.

## 📁 Dataset
- **Name**: Iris Dataset  
- **Source**: Built-in dataset in Scikit-learn  
- **Features**:
  - Sepal Length
  - Sepal Width
  - Petal Length
  - Petal Width  
- **Samples**: 150  
- **Classes**: 3 (Setosa, Versicolor, Virginica)

## 🏗️ Model Architecture
- **Algorithm**: K-Means Clustering  
- **Preprocessing**: MinMaxScaler for feature scaling  
- **Evaluation Tool**: Elbow Method  
- **Visualization**: Scatter plots using matplotlib & seaborn

## 🏋️‍♂️ Training
1. Load and preprocess the Iris dataset.
2. Scale features using MinMaxScaler.
3. Train K-Means model with different cluster sizes.
4. Evaluate using **inertia** values to apply the Elbow method.
5. Fit final model with optimal clusters.

## 📊 Evaluation
- **Elbow Method**: Used to identify the optimal number of clusters (k=3).
- **Visualization**: Scatter plots of features show clear separation between the clusters.

## 🚀 Usage
```bash
# Clone the repository
git clone https://github.com/yourusername/iris-kmeans-clustering.git
cd iris-kmeans-clustering

# Install required libraries
pip install -r requirements.txt

# Run the script
python iris_kmeans.py

📦 Requirements
- Python 3.x
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

🧠 What I Learned
- How to implement K-Means clustering using Scikit-learn.
- The importance of feature scaling in unsupervised learning.
- How to determine optimal cluster count using the Elbow method.
- Gained insights into data visualization techniques for clustering.

🙌 Acknowledgements
- Scikit-learn documentation
- Matplotlib and Seaborn for beautiful visualizations
- The open-source community for inspiration and resources
