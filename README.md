
# 🛡️ Social Media Fake Account Detection

<div align="center">

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/74112721/ccd3a946-ef1b-4ea1-bdae-eafcd7e91691" alt="Social Media Fake Account Detection" width="750"/>

### Detecting Fake Social Media Profiles Using Machine Learning

**A machine learning-based approach to identifying fraudulent social media accounts through profile analysis and classification algorithms.**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Classifier-green)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-ML-yellow?logo=scikitlearn)

</div>

---

## 📖 Overview

Fake social media accounts pose significant challenges to online security, privacy, and digital trust. These accounts may be used for spam, impersonation, misinformation, and fraudulent activities.

This project presents a **machine learning-based fake account detection system** that analyzes social media profile characteristics to distinguish between genuine and fake users.

The system uses profile-related attributes, data preprocessing, feature engineering, and supervised machine learning algorithms to perform classification.

Five machine learning models are explored:

- **Support Vector Machine (SVM)**
- **Random Forest**
- **AdaBoost**
- **XGBoost**
- **Decision Tree**

XGBoost serves as the primary model, while the other algorithms provide comparative evaluation.

---

## ✨ Key Features

- Automated classification of fake and genuine accounts
- Social media profile feature analysis
- Categorical feature encoding and data preprocessing
- Name-based gender prediction as an engineered feature
- Training and evaluation of five ML classifiers
- Cross-validation and learning curve analysis
- Confusion matrix visualization
- Comparative model performance analysis

---

## 🏗️ System Architecture

The proposed system follows a machine learning pipeline, beginning with dataset collection and preprocessing, followed by model training, prediction, and evaluation.

<div align="center">

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/9d008a6c-ce37-40d5-b709-89661a60eafd" alt="System Architecture Diagram" width="850"/>

<br/>

<b>Figure 1: System Architecture of Fake Account Detection</b>

</div>

### Workflow

```text
Social Media Profile Dataset
            |
            v
     Data Preprocessing
            |
            v
     Feature Engineering
            |
            v
      Train-Test Split
            |
            v
   Machine Learning Models
   |    |    |    |    |
  SVM   RF  Ada  XGB   DT
            |
            v
    Prediction & Evaluation
            |
            v
      Fake / Genuine
```

---

## 📊 Dataset Description

The dataset contains social media account information representing both genuine and fake profiles.

The following attributes are used to identify patterns associated with account authenticity.

| Feature | Description |
|---------|-------------|
| Status Count | Number of statuses or posts published |
| Followers Count | Number of followers |
| Friends Count | Number of accounts followed |
| Favorites Count | Number of liked or favorited posts |
| Listed Count | Number of lists containing the account |
| Language | Account's associated language |
| Name | Profile name used for feature engineering |
| Gender | Name-based predicted gender feature |

These features form the input for the classification models.

---

## ⚙️ Methodology

### 1. Data Preprocessing

The dataset undergoes preprocessing to prepare account-level attributes for machine learning.

The process includes:

- Handling and transforming input features
- Encoding categorical attributes such as language
- Generating a name-based gender prediction feature
- Preparing numerical features for model training

### 2. Dataset Splitting

The processed dataset is divided into:

- **Training set:** Used to train machine learning models
- **Testing set:** Used to evaluate model performance on unseen data

### 3. Model Training

Five supervised learning algorithms are considered.

| Algorithm | Description |
|-----------|-------------|
| SVM | Finds a decision boundary to distinguish classes |
| Random Forest | Combines multiple decision trees |
| AdaBoost | Sequentially improves weak learners |
| XGBoost | Uses optimized gradient-boosted trees |
| Decision Tree | Classifies accounts using learned decision rules |

### 4. Model Validation

Cross-validation and learning curves are used to examine model behavior.

**Cross-Validation**

Evaluates how well the model generalizes across different training and validation subsets.

**Learning Curves**

Help identify potential underfitting or overfitting by comparing training and validation performance as training size increases.

---

## 📈 Model Evaluation & Results

The performance of the five machine learning algorithms is evaluated using confusion matrices and classification metrics.

### Confusion Matrix Comparison

The following visualizations show the classification outcomes of all five models.

<div align="center">

<table>
<tr>
<td align="center" width="50%">

<b>Support Vector Machine (SVM)</b>

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/74112721/a2b566e4-fc65-43ba-9232-1b1abab60dc3" width="350" alt="SVM Confusion Matrix"/>

</td>
<td align="center" width="50%">

<b>Random Forest</b>

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/ec9ada62-a915-4dcf-8ce5-6301bd8254cc" width="350" alt="Random Forest Confusion Matrix"/>

</td>
</tr>

<tr>
<td align="center">

<b>AdaBoost</b>

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/19d4f4b3-15e1-409c-b47b-c556401bcd8d" width="350" alt="AdaBoost Confusion Matrix"/>

</td>
<td align="center">

<b>XGBoost</b>

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/458995cd-77ca-41f3-9208-182fd1bd94d2" width="350" alt="XGBoost Confusion Matrix"/>

</td>
</tr>

<tr>
<td align="center" colspan="2">

<b>Decision Tree</b>

<br/>

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/19d4f4b3-15e1-409c-b47b-c556401bcd8d" width="350" alt="Decision Tree Confusion Matrix"/>

</td>
</tr>
</table>

<b>Figure 2: Confusion Matrix Comparison of Five Machine Learning Models</b>

</div>

> **Note:** The original project provides the same image URL for the AdaBoost and Decision Tree confusion matrices. Replace the Decision Tree image URL if a separate visualization is available.

---

## 🔬 Experimental Results and Analysis

The following experimental visualizations provide additional insights into the comparative performance and behavior of the machine learning models.

<div align="center">

<table>
<tr>
<td align="center" width="50%">

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/04d5a737-d2f0-47a4-afc9-0e2c5afac844" width="420" alt="Experimental Result 1"/>

</td>
<td align="center" width="50%">

<img src="https://github.com/Vinod-Ghanchi/Social-Media-Fake-Account-Detection/assets/80514865/80959721-ec8a-4d2b-9bdc-7e929a84d1d3" width="420" alt="Experimental Result 2"/>

</td>
</tr>
</table>

<b>Figure 3: Experimental Results and Performance Analysis</b>

</div>

### Evaluation Metrics

The machine learning classifiers are evaluated based on the following metrics:

| Metric | Purpose |
|--------|---------|
| Accuracy | Measures the proportion of correctly classified accounts |
| Precision | Measures how many predicted fake accounts are actually fake |
| Recall | Measures how many actual fake accounts are successfully identified |
| F1-Score | Balances precision and recall |
| Confusion Matrix | Displays correct and incorrect predictions for each class |

The confusion matrix provides four classification outcomes:

- **True Positive (TP):** Fake account correctly classified as fake
- **True Negative (TN):** Genuine account correctly classified as genuine
- **False Positive (FP):** Genuine account incorrectly classified as fake
- **False Negative (FN):** Fake account incorrectly classified as genuine

These metrics support a more comprehensive evaluation than classification accuracy alone.

---

## 🧠 Why XGBoost?

XGBoost (Extreme Gradient Boosting) is the primary machine learning model explored in this project.

It offers several advantages:

- Efficient gradient-boosted decision tree training
- Ability to capture complex feature relationships
- Regularization to help reduce overfitting
- Support for feature importance analysis
- Strong performance on many structured datasets

The comparative evaluation with SVM, Random Forest, AdaBoost, and Decision Tree provides a basis for assessing its effectiveness.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming language |
| Pandas | Data manipulation and preprocessing |
| NumPy | Numerical computation |
| Scikit-learn | Machine learning and evaluation |
| XGBoost | Gradient boosting classifier |
| Matplotlib | Data visualization |
| Seaborn | Statistical plotting |

---

## 🎯 Applications

This fake account detection approach may be useful for:

- Social media account authenticity analysis
- Spam and bot detection research
- Fraudulent profile identification
- Online security research
- Machine learning classification benchmarking

---

## 🚀 Future Enhancements

Potential improvements to the project include:

1. **Deep Learning Integration** — Explore neural networks for more complex behavioral patterns.
2. **Real-Time Detection** — Develop a system for classifying accounts from live profile data.
3. **Advanced Feature Engineering** — Include account age, engagement ratios, and posting frequency.
4. **Hyperparameter Optimization** — Tune models to improve generalization performance.
5. **Explainable AI** — Integrate SHAP or similar methods to interpret predictions.
6. **Web Application** — Build a user-friendly interface for account analysis.

---

## 📌 Conclusion

This project demonstrates the application of supervised machine learning techniques for detecting fake social media accounts using profile-based features.

By implementing and evaluating **SVM, Random Forest, AdaBoost, XGBoost, and Decision Tree**, the system establishes a comparative framework for identifying suspicious accounts.

The use of preprocessing, feature engineering, cross-validation, and multiple performance metrics supports systematic model evaluation.

Further improvements can strengthen the system's reliability, interpretability, and suitability for real-world applications.

---

<div align="center">

### 🛡️ Building Safer Social Media Platforms Through Machine Learning

**If you find this project useful, consider giving it a ⭐!**

</div>
