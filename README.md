# Human Activity Recognition using Random Forest (KNIME)

This project implements a Human Activity Recognition (HAR) classification workflow using the KNIME Analytics Platform and a Random Forest model.

The goal is to classify human activities based on smartphone sensor data.

---

## Dataset

The dataset used in this project is the **Human Activity Recognition Using Smartphones Dataset**, publicly available from the UCI Machine Learning Repository.

### Source
- UCI Machine Learning Repository  
- Dataset name: *Human Activity Recognition Using Smartphones*  
- URL: https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones

### Description
The data was collected from 30 subjects performing daily activities while carrying a smartphone (Samsung Galaxy S II) on the waist.  
The smartphone's accelerometer and gyroscope captured motion signals.

Activities include:
- Walking
- Walking Upstairs
- Walking Downstairs
- Sitting
- Standing
- Laying

### Files used
- `X_train.txt` – training feature vectors
- `y_train.txt` – activity labels (numeric)
- `activity_labels.txt` – mapping of numeric labels to activity names

The dataset files are **not included** in this repository due to size and licensing considerations.  
To run the workflow, the dataset must be downloaded separately and placed in the local KNIME workspace.

---

## Workflow Overview

The KNIME workflow performs the following steps:

1. Load feature data (`X_train`)
2. Load activity labels (`y_train`)
3. Map numeric activity IDs to descriptive activity names
4. Merge features and labels using Joiner nodes
5. Split the data into training (70%) and testing (30%) sets
6. Train a Random Forest classifier
7. Predict activities on the test set
8. Evaluate the model using a Scorer node (accuracy and confusion matrix)

---

## Tools and Technologies

- KNIME Analytics Platform (version 5.x)
- Random Forest (classification)
- Java (required by KNIME)

---

## Repository Contents

- `Human_Activity_Recognition.knwf` – KNIME workflow file
- `README.md` – project documentation
- `LICENSE` – MIT License

---

## License

This project is licensed under the MIT License.
