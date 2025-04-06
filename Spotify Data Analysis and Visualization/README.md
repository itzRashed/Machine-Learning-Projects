# 🎧 Spotify Data Analysis and Visualization  
This project explores and analyzes the **Spotify 2023 dataset** to gain insights into music trends, song characteristics, and listener preferences. It includes data cleaning, visualization, normalization, and dimensionality reduction techniques such as **PCA** to uncover meaningful patterns and relationships between features.

> 📍 Implemented in Jupyter Notebook – `Spotify Data Analysis and Visualization.ipynb`

## 📌 Project Overview  
The project aims to identify patterns in Spotify music data by applying various **data mining and machine learning techniques**. By reducing the feature space using PCA, we are able to visualize and understand song characteristics that contribute to their popularity.

## 📂 Dataset  
- The dataset used is the publicly available **Spotify 2023 dataset**  
- Includes features like danceability, energy, tempo, etc. for each track  
- Used for clustering and popularity prediction  

## ⚙️ Dependencies  
Install the following Python libraries:
```bash
pip install pandas matplotlib numpy scikit-learn seaborn

🧠 Methodology
🔹 Data Loading and Cleaning
- Loaded the dataset using pandas
- Removed rows with missing values
- Dropped duplicate entries to maintain data quality

🔹 Data Exploration & Visualization
- Inspected dataset using df.info() and df.describe()
- Created visualizations including:
 📊 Box plots
 📈 Histograms
- Identified and removed outliers using Z-score analysis

🔹 Data Sampling & Discretization
- Performed random sampling using df.sample()
- Discretized continuous features using pd.cut() and pd.qcut()

🔹 Data Normalization
- Applied Min-Max Scaling to normalize feature values

🔹 Principal Component Analysis (PCA)
- Conducted PCA for dimensionality reduction
- Visualized principal components using 2D scatter plots

📊 Results
- 📈 A positive correlation was observed between song energy and Spotify chart performance
- 🧬 First two principal components captured a significant portion of variance
- 🎶 Popular songs typically had higher energy, danceability, and tempo

⚠️ Limitations
- Dataset may not fully represent all genres or global regions
- Cultural and lyrical elements are not captured
- Focus is limited to numerical audio features, which may not reflect subjective popularity

🚀 Future Work
-  Apply K-Means clustering to group similar songs
- Use regression models to predict popularity scores
- Expand analysis with multi-year Spotify datasets for trend detection

🛠️ Usage
To run the project locally:
Clone the repository

```bash
git clone https://github.com/your-username/spotify-data-analysis.git

Navigate to the project folder
```bash
cd spotify-data-analysis
Install the required dependencies (see above)

Launch the Jupyter Notebook
```bash
jupyter notebook Spotify Data Analysis and Visualization.ipynb

🤝 Contributing
Contributions are welcome!
If you have ideas or improvements, feel free to open an issue or submit a pull request.

📄 License
This project is licensed under the MIT License
