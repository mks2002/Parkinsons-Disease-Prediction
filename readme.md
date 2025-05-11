

# Parkinson's Disease Prediction

This project applies machine learning techniques to predict Parkinson's Disease using a biomedical dataset. Several classifiers, including **Support Vector Machines (SVM)** and **Random Forest**, are implemented and compared for their performance in predicting the disease.

## Table of Contents

- [Project Structure](#project-structure)
- [Models Implemented](#models-implemented)
- [Dataset](#dataset)
- [Model Performance](#model-performance)
- [Requirements](#requirements)
- [Usage](#usage)
- [Contribution](#contribution)
- [Model Comparison and Insights](#model-comparison-and-insights)
- [Acknowledgments](#acknowledgments)

## Project Structure

This repository contains the following Jupyter notebooks:

1. **comparison.ipynb**: Compares the performance of multiple classifiers (SVM, Random Forest, MLP, KNN, Naive Bayes, GBM) for Parkinson's Disease prediction.
2. **svm.ipynb**: Focuses on the implementation and evaluation of the SVM classifier for the Parkinson's Disease prediction task.

## Models Implemented

- **Support Vector Machine (SVM)**
- **Random Forest**
- **Multi-Layer Perceptron (MLP)**
- **K-Nearest Neighbors (KNN)**
- **Naive Bayes**
- **Gradient Boosting Machines (GBM)**

## Dataset

The dataset consists of 195 records from 31 patients, with 22 voice-related biomedical features that are used for diagnosing Parkinson's Disease. The target variable (`status`) is binary:

- **1**: The patient has Parkinson's Disease.
- **0**: The patient does not have Parkinson's Disease.

More details about the dataset can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Parkinsons).

## Model Performance

After training and evaluating different machine learning models, the performance metrics were as follows:

| Model                        | Accuracy | Precision | Recall | F1-Score |
| ---------------------------- | -------- | --------- | ------ | -------- |
| SVM                          | 87.17%   | 87.5%     | 88.6%  | 87.9%    |
| Random Forest                | 87.17%   | 87.5%     | 88.6%  | 87.9%    |
| Multi-Layer Perceptron (MLP) | 84.61%   | 84.9%     | 85.2%  | 84.8%    |
| K-Nearest Neighbors (KNN)    | 82.56%   | 82.3%     | 83.5%  | 82.9%    |
| Naive Bayes                  | 79.48%   | 79.2%     | 80.3%  | 79.7%    |

Random Forest and SVM both achieved the highest accuracy of **87.17%**, demonstrating their effectiveness in predicting Parkinson's Disease based on the given dataset.

## Requirements

To run the notebooks, install the required dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

Contents of `requirements.txt`:

```txt
numpy
pandas
matplotlib
scikit-learn
seaborn
jupyterlab
```

## Usage

1. Clone the repository:
   ```bash
   git clone Parkinsons-Disease-Prediction
   ```
2. Navigate to the project directory:
   ```bash
   cd Parkinsons-Disease-Prediction
   ```
3. Open the Jupyter notebooks:
   ```bash
   jupyter notebook
   ```
4. Open either `comparison.ipynb` or `svm.ipynb` and run the cells to see model training and evaluation results.

## Contribution

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m "Added feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request detailing your changes.

## Model Comparison and Insights

In the **comparison.ipynb** notebook, we explored multiple models, and the results showed that both SVM and Random Forest provided the best balance between precision, recall, and overall accuracy.

This highlights the robustness of ensemble methods like Random Forest as well as the potential of linear classifiers such as SVM for tasks involving a binary classification problem with clear decision boundaries.

The **svm.ipynb** notebook provides further insight into the effectiveness of SVM for this task. The use of SVM's hyperparameters, including kernel types and regularization, is thoroughly explored.

## Acknowledgments

- **UCI Machine Learning Repository** for providing the dataset.
- Thanks to the open-source community for making these libraries and tools available.
