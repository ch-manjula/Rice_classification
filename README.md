# 🌾 Rice Type Classification Using Machine Learning

## 📌 Brief Description

This project aims to classify different types of rice grains using machine learning algorithms and deploys the solution via a **Streamlit web application**. By analyzing physical attributes of rice grains—such as area, perimeter, axis lengths, and eccentricity—the model classifies grains into one of three categories: **Cammeo**, **Jasmine**

Several ML algorithms were evaluated, including **SVM**, **KNN**, and **Decision Tree**, with **Support Vector Machine (SVM)** achieving the highest classification accuracy (~96%). The best-performing model is integrated into a **Streamlit app**, where users can input feature values and receive real-time rice type predictions. A test run in the app correctly identified the rice type, validating the pipeline.

---

## 📁 Directory Structure

rice-classification-ml/
│
├── rice_finalproject.ipynb # Jupyter Notebook for data preprocessing and model training
├── ricetext.ipynb # Streamlit logic in notebook format
├── Screenshot 2025-06-19.png # Streamlit app showing correct rice prediction
├── app.py # (Optional) Converted Streamlit app for deployment
├── requirements.txt # Required Python libraries
├── README.md # Project documentation (this file)
└── rice_dataset.csv # (Optional) Dataset (if included locally)


> 💡 You can export `ricetext.ipynb` to `app.py` using Jupyter or `nbconvert` to run it with Streamlit.

---

## 🧠 Problem Statement

Manual classification of rice grains is inefficient, prone to human error, and unsuitable for large-scale use. This project proposes an automated system using machine learning to classify rice grains based on measurable physical features, improving accuracy and speed.

---

## 🔬 Literature Review

- Previous research shows SVM and KNN work well with small but high-quality feature datasets.
- CNNs work well with image data but require extensive data and resources.
- Feature-based models combined with simple classifiers offer a practical solution with good accuracy and low computational needs.

---

## ✅ Proposed Solution

1. Collect and preprocess morphological rice grain data.
2. Analyze feature distributions and correlations.
3. Train and evaluate machine learning classifiers.
4. Deploy the best model using Streamlit for real-time predictions.

---

## ⚙️ Algorithms Used

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree Classifier

---

## 📁 Dataset Description

- **Source:** UCI Machine Learning Repository – Rice Dataset  
- **Target Classes:**  
  - Cammeo  
  - Jasmine  
  - Karacadag  
- **Features Used:**
  - Area
  - Perimeter
  - MajorAxisLength
  - MinorAxisLength
  - Eccentricity
  - ConvexArea
  - EquivalentDiameter
  - Extent
  - Solidity

---

## 📊 Results and Discussion

| Model                | Accuracy |
|---------------------|----------|
| K-Nearest Neighbors | ~95%     |
| Support Vector Machine | ~96%  |
| Decision Tree        | ~93%     |

- **SVM** outperformed other models, demonstrating better generalization.
- Feature scaling was essential for models like SVM and KNN.
- Confusion matrix showed minimal overlap between classes.

---

## 💻 Streamlit Web App

The best-performing model is deployed in a **Streamlit web app** allowing users to input feature values and receive predictions instantly.

### 🔍 Prediction Example:

- The attached screenshot (`Screenshot 2025-06-19.png`) shows a successful prediction by the app.
- Inputted values led to the correct classification, demonstrating the system's real-world usability.

### ▶️ How to Run the App
Go to anaconda prompt 
Give the necessary file path and enter 
Give streamlit app name 

streamlit run app.py



