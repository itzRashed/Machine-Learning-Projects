# 📝 Sentiment Analyzer
This project is a **Sentiment Analysis Tool** built with **Python** and **scikit-learn**, designed to classify customer reviews as **positive** or **negative** using a **Support Vector Machine (SVM)** model.

## 🎯 Overview
The aim of this project is to develop a machine learning model that can accurately analyze and classify the sentiment of customer reviews. It includes text preprocessing, model training, performance evaluation, and visualization of results.

## 📁 Dataset

- **Name**: Reviews.csv  
- **Source**: [Public dataset of customer reviews]  
- **Contents**:
  - Customer reviews  
  - Associated review scores  
- **Labeling**:
  - Score > 3 → **Positive**  
  - Score ≤ 3 → **Negative**

## 🧠 Methodology
1. **Data Loading & Preprocessing**  
   - Loaded using `pandas`  
   - Labeled reviews as positive or negative  
   - Removed stop words and vectorized text using **TF-IDF**

2. **Model Training**  
   - Used **Support Vector Machine (SVM)** with a linear kernel  
   - Data split into training and testing sets (e.g., 80/20)

3. **Model Evaluation**  
   - Evaluated with:
     - Accuracy
     - Confusion Matrix
     - Classification Report
     - ROC Curve

4. **Visualization**  
   - Plotted confusion matrix and ROC curve using `matplotlib` and `seaborn`

## 🚀 Usage
```bash
# Clone the repository
git clone https://github.com/yourusername/sentiment-analyzer.git
cd sentiment-analyzer

# Install required packages
pip install pandas scikit-learn matplotlib seaborn

# Run the project
python sentiment_analyzer.py
📊 Results
- The model achieves an accuracy of [insert accuracy score here]% on the test set.
- The confusion matrix and ROC curve demonstrate the model’s ability to distinguish between positive and negative reviews.

🧠 What I Learned
- Implementing an end-to-end text classification pipeline
- Importance of text preprocessing in NLP tasks
- Evaluating ML models using proper classification metrics
- Visualizing results for better interpretation

🙌 Acknowledgements
- scikit-learn documentation
- Matplotlib & Seaborn libraries
- Community contributors and open-source resources


