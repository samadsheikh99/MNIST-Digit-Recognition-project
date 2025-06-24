# 🧠 MNIST Digit Recognition using Scikit-learn

This project implements a complete classification pipeline for recognizing handwritten digits from the MNIST dataset using Scikit-learn. The task explores fundamental classification concepts and compares performance between key classifiers like SGD and Random Forest, including evaluation with visual analysis and a web interface.

## 📌 Objectives

- Understand and apply core classification techniques.
- Evaluate classifier performance with precision, recall, F1, and confusion matrix.
- Visualize and analyze common classification errors.
- Build a Gradio web app for real-time digit recognition.
- Achieve minimum 95% test accuracy on MNIST.

## 📚 Key Topics (from Chapter 3 of "Hands-On ML")

- Binary vs Multiclass Classification
- Confusion Matrix, Precision/Recall, F1 Score
- ROC Curves and Decision Thresholds
- Multioutput and Multilabel Classification
- Error Analysis and Model Optimization

## 🗃️ Dataset

- **MNIST 784** dataset (handwritten digits)
- Source: [Kaggle / OpenML](https://www.openml.org/d/554)

Each image is 28x28 grayscale (784 features) representing digits 0–9.

## 🛠️ Implementation Steps

1. **Data Loading**  
   - Load MNIST dataset using `fetch_openml("mnist_784")`.

2. **Data Preprocessing**  
   - Split into train (60K) and test (10K) sets.
   - Normalize pixel values.

3. **Train Classifiers**  
   - `SGDClassifier` with hinge loss (SVM-like).
   - `RandomForestClassifier`.

4. **Model Evaluation**  
   - Use confusion matrix and classification report.
   - Visualize worst misclassifications.
   - Plot precision-recall and ROC curves.

5. **Error Analysis**  
   - Identify systematic misclassifications (e.g. 9 vs 4).
   - Propose improvements (e.g., image sharpening, more data).

6. **Deployment (Optional)**  
   - Build a Gradio web interface to classify digits drawn by users.

## 🧪 Classifier Comparison

| Classifier        | Accuracy | Precision | Recall | F1 Score |
|-------------------|----------|-----------|--------|----------|
| SGD Classifier    | 91.7%    | 91.5%     | 91.7%  | 91.6%    |
| Random Forest     | 96.8%    | 96.9%     | 96.8%  | 96.8%    |

## 🖼️ Visual Examples

Misclassified digit pairs (e.g., 9 → 4, 7 → 1) are visualized using matplotlib to better understand model limitations.

## 🚀 Web App

The model is integrated into a `Gradio` web app allowing users to draw digits in real-time and see predictions instantly.

## 📈 Learning Outcomes

- Practical understanding of multiclass classification and performance metrics.
- Ability to diagnose and improve model behavior using error analysis.
- Experience deploying ML models as interactive apps.



 
