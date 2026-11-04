# Practical-Assignment-5-Ensemble-Learning-and-Performance-Evaluation
Implementation and performance comparison of five base classifiers and three ensemble learning techniques (AdaBoost, Voting, and Stacking) using the Rice Classification Dataset with Python and Scikit-learn.

**Rice Classification Using Logistic Regression, Decision Tree, Random Forest, KNN, SVM, AdaBoost, Voting, and Stacking**

Rice classification using Python, Scikit-learn, data preprocessing, exploratory data analysis, ensemble learning, model evaluation, and visualizations.

---

## **1. Introduction**

This practical assignment focuses on implementing and comparing supervised machine learning classification algorithms using Python. The Rice Classification dataset is used to classify rice grains into two categories based on their physical measurements.

The main aim is to understand ensemble learning techniques and compare individual classifiers with ensemble models using appropriate classification metrics.

---

## **2. Objectives**

- Understand the concept and working of ensemble learning.
- Load, inspect, and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Select suitable input features and target variables.
- Implement five base classification algorithms.
- Apply AdaBoost, Voting, and Stacking ensemble techniques.
- Evaluate models using appropriate classification metrics.
- Visualize and compare model performance.
- Identify the best-performing model based on experimental results.

---

## **3. Dataset Description**

The project uses the Rice Classification dataset, which contains physical measurements of rice grains.

**Dataset File:** `riceClassification.csv`

The dataset contains 18,185 records and 12 columns, including an identifier, numerical features, and the target class.

**Features Used for Classification:**

- `Area`
- `MajorAxisLength`
- `MinorAxisLength`
- `Eccentricity`
- `ConvexArea`
- `EquivDiameter`
- `Extent`
- `Perimeter`
- `Roundness`
- `AspectRation`

**Target Variable:** `Class`

The `id` column is excluded from model training because it is only an identifier. The target variable contains two classes: 0 and 1.

---

## **4. Algorithms Used**

### **4.1 Logistic Regression**

Logistic Regression is a supervised classification algorithm that predicts the probability of an observation belonging to a particular class.

### **4.2 Decision Tree**

Decision Tree is a tree-based classification algorithm that makes predictions using a sequence of feature-based decisions.

### **4.3 Random Forest**

Random Forest combines multiple decision trees and uses their predictions to produce the final classification result.

### **4.4 K-Nearest Neighbors (KNN)**

KNN classifies a data point based on the majority class among its nearest neighbors.

### **4.5 Support Vector Machine (SVM)**

SVM identifies an optimal decision boundary that separates different classes in the feature space.

### **4.6 AdaBoost Ensemble**

AdaBoost is a boosting technique that combines weak learners sequentially and gives greater importance to incorrectly classified observations during training.

### **4.7 Voting Ensemble**

Voting combines predictions from multiple classifiers. This project uses Hard Voting, where the class receiving the majority of votes becomes the final prediction.

### **4.8 Stacking Ensemble**

Stacking combines predictions from multiple base classifiers using a meta-classifier. In this project, Logistic Regression is used as the meta-classifier.

---

## **5. Tools and Technologies**

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook or JupyterLab

---

## **6. Implementation Steps**

1. Load and inspect the Rice Classification dataset.
2. Check missing values, duplicate records, data types, and statistical summaries.
3. Perform exploratory data analysis using count plots, histograms, box plots, and correlation heatmaps.
4. Select numerical input features and the target variable.
5. Exclude the identifier column from model training.
6. Split the dataset into training and testing sets using an 80:20 ratio.
7. Apply median imputation and feature scaling using StandardScaler.
8. Train five base classifiers: Logistic Regression, Decision Tree, Random Forest, KNN, and SVM.
9. Implement AdaBoost using a Decision Tree with maximum depth 1 as the weak learner.
10. Implement Voting using Hard Voting.
11. Implement Stacking using Logistic Regression as the meta-classifier.
12. Evaluate all eight models using classification metrics.
13. Generate performance comparison graphs, confusion matrices, and classification reports.
14. Compare the results and identify the best-performing model.

---

## **7. Evaluation Metrics**

- **Accuracy:** Measures the proportion of correctly classified predictions.
- **Precision:** Measures how many positive predictions are actually positive.
- **Recall:** Measures how many actual positive observations are correctly identified.
- **F1-Score:** Represents the harmonic mean of Precision and Recall.
- **ROC-AUC:** Measures the model's ability to distinguish between the two classes.
- **Balanced Accuracy:** Calculates the average recall obtained across the classes.

Macro averaging is used for Precision, Recall, and F1-Score to give equal importance to both classes.

For Hard Voting, ROC-AUC is reported as N/A because the classifier produces class predictions rather than probability scores.

---

## **8. Results and Comparative Analysis**

The five base classifiers and three ensemble models are compared using Accuracy, Precision, Recall, F1-Score, ROC-AUC, and Balanced Accuracy.

The experimental results are used to identify the best-performing model.

Based on the recorded notebook results, Stacking achieved the highest performance among the eight models.

- **Best Model:** Stacking Ensemble
- **Accuracy:** 99.37%
- **Macro F1-Score:** 0.9936
- **ROC-AUC:** 0.9993

Performance comparison graphs and confusion matrices help visualize the classification results.

---

## **9. How to Run the Project**

### **Step 1: Install the Required Libraries**

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### **Step 2: Keep the Files Together**

Place the following files in the same directory:

- `Practical_Assignment_5_Exact_Code_One_Cell.ipynb`
- `riceClassification.csv`

### **Step 3: Start Jupyter Notebook**

```bash
jupyter notebook
```

Open the notebook and run the code cell. The notebook can be executed using Jupyter Notebook or JupyterLab.

---

## **10. Output and Visualizations**

After successful execution, the notebook generates:

- Dataset information and statistical summaries.
- Rice class distribution plot.
- Feature distribution histograms.
- Feature box plots.
- Correlation heatmap.
- Model performance comparison graphs.
- Confusion matrices for all eight models.
- Classification reports.
- Final model comparison table.

---

## **11. Conclusion**

This practical demonstrates the implementation and comparison of five base classification algorithms and three ensemble learning techniques: AdaBoost, Voting, and Stacking.

The models are trained and evaluated using the Rice Classification dataset. The experimental results show that Stacking achieved the highest accuracy and Macro F1-Score among the evaluated models.

This practical helps understand how ensemble learning combines multiple classifiers and how classification metrics can be used to identify a suitable machine learning model.

---

## **12. Author**

**Tushar Vijay Chaudhari**

- **Institution:** MIT Academy of Engineering (MIT AOE), Alandi, Pune
- **Department:** Electronics and Telecommunication Engineering (ENTC)
- **Assignment:** Practical Assignment 5 — Ensemble Learning and Performance Evaluation
