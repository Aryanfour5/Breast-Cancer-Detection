Breast Cancer Prediction using SVM Classifier

This repository contains a Python script that demonstrates how to train a Support Vector Machine (SVM) classifier with a linear kernel to predict breast cancer based on features extracted from biopsy samples. It also evaluates the accuracy of the classifier on a test dataset.
Dataset

The dataset used in this script is sourced from the UCI Machine Learning Repository. It consists of diagnostic measurements for breast cancer and includes the following features:

    Features:
        clump_thickness
        uniform_cell_size
        uniform_cell_shape
        marginal_adhesion
        single_epithelial_size
        bare_nuclei
        bland_chromatin
        normal_nucleoli
        mitoses

    Target Variable:
        class (2 for benign, 4 for malignant)

Installation

    Clone the repository:

    bash

git clone <repository_url>
cd <repository_name>

Install the required Python libraries:

bash

pip install numpy pandas matplotlib scikit-learn

Run the script:

bash

    python breast_cancer_prediction.py

Usage

    Data Preprocessing:

    The dataset is preprocessed by replacing missing values ('?') with -99999 and dropping the 'id' column.

    Exploratory Data Analysis:
        Summary statistics of the dataset are displayed using df.describe().
        Histograms and scatter matrix plots are generated for data visualization.

    Model Training and Evaluation:

        Two models are evaluated:
            K-Nearest Neighbors (KNN) Classifier
            Support Vector Machine (SVM) Classifier with linear kernel

        Cross-validation is used to assess model performance:
            Accuracy scores and standard deviations are printed for each model.

        Performance metrics (precision, recall, F1-score) and confusion matrices are generated for both models on the test set.

Results

After evaluating the SVM classifier with a linear kernel on a test set:

    Accuracy on test set: 1.00

    Predictions:
        Sample 1: Predicted to not have cancer
        Sample 2: Predicted to have cancer



    Dataset source: UCI Machine Learning Repository
