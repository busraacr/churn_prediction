# Customer Churn Prediction with Machine Learning

## 📌 Project Overview

This project aims to predict **customer churn** using a machine learning pipeline, addressing **class imbalance** with various **resampling techniques** and evaluating model performance using multiple **classification algorithms**.

### **🔍 Key Features**

- **Data Preprocessing**: Handling missing values, encoding categorical variables, normalization, feature selection.
- **Resampling Techniques**: SMOTE, Borderline-SMOTE, ADASYN, Random Oversampling (ROS), Random Undersampling (RUS), SMOTE-Tomek.
- **Machine Learning Models**: Logistic Regression, Decision Tree, Random Forest, SVM, XGBoost, KNN, Naive Bayes.
- **Evaluation Metrics**: PR-AUC, ROC-AUC, Accuracy, Confusion Matrix, Precision-Recall Curve.
- **Performance Comparisons**: Unified results stored for ranking top-performing models.

---

## 🛠 Installation & Setup

### **1️. Clone the Repository**

```bash
git clone https://github.com/busraacr/churn_prediction.git
cd churn_prediction
```

### **2. Install Dependencies**

This project requires several Python libraries for preprocessing, model training, and visualization. Run the following command to install all dependencies:

```bash
pip install -r requirements.txt
```

### **3. Running Jupyter Notebooks**

Since this project contains Jupyter Notebooks (.ipynb), you need to install Jupyter and run the notebooks interactively. To install Jupyter:

```bash
pip install notebook
```

Start Jupyter Notebook with:

```bash
jupyter notebook
```

Then navigate to the folder containing the .ipynb files and open them.

### **4. Run Preprocessing**

Open and execute:

```bash
notebooks/preprocessing.ipynb
```

The prepossesed data is saved in the data/filtered_data file for future usage.

### **5. Apply Resampling**

Each resampling technique is applied **individually** to the filtered dataset to address class imbalance. The processed datasets are then saved in the `data/resampled_data/` folder for further analysis.

### **6. Train Machine Learning Models**

The resampled datasets are used to train multiple machine learning models, ensuring a comparative analysis of their performance across different resampling methods.

### **7. View and Compare Results**

Final model comparison results are available in the following Jupyter Notebook:

```bash
notebooks/ml_comparison.ipynb
```

## 📈 Visual Representations

The following plots support analysis:

- **Feature Correlation Heatmap**: Identifies key predictors of churn.

- **Pie Chart**: Visualizes class imbalance.

- **Bar Chart**: Ranks the top-performing models by PR-AUC.

- **Sankey Diagram**: Shows the flow of models through score categories.

- **Scatter Plot**: Illustrates PR-AUC vs Accuracy trends.
