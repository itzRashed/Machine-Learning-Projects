🎧 Spotify Data Analysis and Visualization
📌 Project Overview
This project explores and analyzes the Spotify 2023 dataset to gain insights into music trends, song characteristics, and patterns in listener preferences. Through data cleaning, visualization, normalization, and dimensionality reduction techniques like PCA, we uncover relationships between features and provide meaningful data-driven insights.

📂 Dataset
The dataset used is the publicly available Spotify 2023 dataset.
🔗 Access the dataset here

⚙️ Dependencies
Ensure you have the following Python libraries installed:
bash: pip install pandas matplotlib numpy scikit-learn seaborn

🧠 Methodology
1. Data Loading and Cleaning
- Loaded the dataset using pandas.
- Removed rows with missing values.
- Dropped duplicate entries to ensure data quality.

2. Data Exploration & Visualization
- Inspected the dataset using df.info() and df.describe().
- Created visualizations including:
📊 Box plots
📈 Histograms
- Identified and removed outliers using Z-score analysis.

3. Data Sampling & Discretization
- Performed random sampling with df.sample() for efficient analysis.
- Discretized numerical values using pd.cut() and pd.qcut().

4. Data Normalization
- Applied Min-Max Scaling to normalize feature values before PCA.

5. Principal Component Analysis (PCA)
- Conducted PCA to reduce dimensionality.
- Visualized principal components using 2D scatter plots.

📊 Results
- 📈 A positive correlation was observed between song energy and Spotify chart performance.
- 🧬 The first two principal components explained a large portion of variance in the dataset.
- 🎶 Popular songs generally had higher energy, danceability, and tempo.

⚠️ Limitations
- The dataset may not be equally representative of all genres or regions.
- Some cultural and lyrical features are not included in the data.
- Focuses primarily on numerical audio features, which may miss subjective aspects of popularity.

🚀 Future Work
- Implement clustering techniques (e.g., K-Means) to find natural groupings of songs.
- Apply regression models to predict song popularity metrics.
- Expand the analysis with multi-year Spotify datasets to observe trend changes over time.

🛠️ Usage
To run the project locally:
1. Clone the repository:
bash: git clone https://github.com/your-username/spotify-data-analysis.git
2. Navigate to the project folder:
bash: cd spotify-data-analysis
3. Install the dependencies (see above).
4. Open and run the notebook:
bash: Spotify Data Analysis and Visualization.ipynb

🤝 Contributing
Contributions are welcome!
If you have suggestions or improvements, feel free to open an issue or submit a pull request.

📄 License
This project is licensed under the MIT License.
