# **Breast Cancer Classification using Machine Learning**

## **Overview**
This repository contains the implementation of machine learning models for **breast cancer classification** using the **Breast Cancer Wisconsin (Diagnostic) dataset**. The models included are:
- **Support Vector Machine (SVM)** (primary model)
- **Random Forest Classifier**
- **Gradient Boosting Classifier**
- **K-Nearest Neighbors (KNN)** (included in Option A)

## **Dataset**
The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). It contains **30 numerical features** extracted from digitized images of breast masses, classified as either **malignant (0)** or **benign (1)**.

## **Project Structure**
- **Jupyter Notebook** containing all implementation steps.
- **Python scripts** for each model: SVM, Random Forest, Gradient Boosting, and KNN.
- **Dataset folder** (if applicable).
- **Reports summarizing Option A and Option B analyses.**
- **README file** for project documentation.

## **Installation & Dependencies**
To run this project, install the necessary dependencies using:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

## **Model Implementation**

### **Data Preprocessing**
- **Data is loaded and cleaned.**
- **Features are standardized** using `StandardScaler`.
- **The dataset is split** into 80% training and 20% testing.

### **Hyperparameter Tuning**
- **SVM:** `RandomizedSearchCV` is used to optimize `C`, `kernel`, and `gamma`.
- **Random Forest & Gradient Boosting:** `GridSearchCV` is used for hyperparameter tuning.
- **KNN:** Implemented with `k=5` for baseline comparison.

### **Evaluation Metrics**
- **Accuracy**: Measures the proportion of correct classifications.
- **Precision**: Determines the proportion of correctly predicted positive cases.
- **Recall**: Assesses the ability to identify all relevant positive instances.
- **F1-Score**: Balances precision and recall.

## **Explanation of Evaluation Metrics**
- **Accuracy**: Represents how often the model correctly classifies instances. High accuracy suggests reliable performance.
- **Precision**: Ensures that positive predictions are truly positive, minimizing false positives.
- **Recall**: Prioritizes identifying actual positive cases, which is crucial in medical applications.
- **F1-Score**: Provides a balanced metric between precision and recall, ensuring robust performance.



## **Conclusion**
This project successfully demonstrates the application of machine learning models for breast cancer classification. The **SVM model** was optimized using hyperparameter tuning, and additional models like **Random Forest, Gradient Boosting, and KNN** were evaluated for comparison. The high accuracy and recall rates indicate the potential of these models in medical diagnosis. Further improvements can be made by integrating deep learning techniques and expanding the dataset for more robust performance.
