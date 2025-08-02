

# Student Performance Prediction

This repository contains a machine learning project developed to predict student academic outcomes—specifically, whether a student is likely to pass or fail—based on academic scores, attendance, and study habits. The project was implemented using Python and trained in Google Colab as part of the submission for the IIT Patna Microtek Project Board.

## Project Objective

The objective of this project is to build a predictive model that can assess a student's likelihood of academic success using measurable features such as subject-wise marks, attendance percentage, and study hours. This model may be helpful for identifying at-risk students early and taking corrective academic support measures.

## Dataset Summary

The dataset used contains records of 15 students, with each record representing:

* Subject scores: Math, Physics, Chemistry, Biology, English
* Attendance percentage
* Average study hours per day
* Final result (Pass/Fail)

The target variable is ‘Final\_Result’, which was converted to binary format for modeling: Pass = 1, Fail = 0.

### Sample Data (First Few Entries):

| ID | Math | Physics | Chemistry | Biology | English | Attendance | Hours\_Study | Final\_Result |
| -- | ---- | ------- | --------- | ------- | ------- | ---------- | ------------ | ------------- |
| 1  | 45   | 55      | 52        | 50      | 61      | 75         | 2            | Fail          |
| 2  | 89   | 91      | 94        | 88      | 85      | 92         | 6            | Pass          |
| 3  | 66   | 62      | 70        | 72      | 68      | 80         | 4            | Pass          |

The complete dataset can be found in the student\_data.csv file in this repository.

## Methodology

The project follows a standard supervised learning pipeline:

1. Data loading and exploration using pandas
2. Preprocessing:

   * Removal of unnecessary identifiers (e.g., ID)
   * Label encoding of target variable
   * Ensuring no missing values
3. Splitting of data into training and testing sets
4. Model selection and training using Random Forest Classifier
5. Evaluation using accuracy score and classification metrics

## Model Overview

* Algorithm: Random Forest Classifier
* Number of trees (n\_estimators): 100
* Random state: 42
* Evaluation metrics: Accuracy, Precision, Recall, F1-score

## Results

The model achieved the following results on the test set:

* Accuracy: 1.00
* Precision and recall for both classes were 1.00
* Classification report confirmed perfect predictions on the given dataset

It is worth noting that the dataset is small, and while the model performed well on this data, performance may vary with larger or more diverse datasets.

## Files Included

* Student\_Prediction\_Project.ipynb – Colab notebook with the full code
* student\_data.csv – Dataset used
* README.md – This file
* LICENSE – MIT License

## How to Use

1. Clone the repository to your local machine.
2. Open the Colab notebook using Google Colab.
3. Upload or link the dataset if necessary.
4. Run the notebook step-by-step to train and test the model.

## Future Scope

To improve the robustness and generalizability of the model, the following extensions are recommended:

* Collecting a larger and more diverse dataset
* Applying feature selection or dimensionality reduction
* Evaluating with cross-validation and hyperparameter tuning
* Exploring ensemble models or deep learning architectures





