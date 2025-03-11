# neural-network-challenge-2
# Neural Network Challenge 2

## Overview
This project aims to develop a branched neural network that predicts two outcomes:
1. **Employee Attrition** — Predict whether an employee is likely to leave the company.
2. **Department Recommendation** — Predict the department where an employee best fits.

The model leverages data preprocessing techniques and a branched neural network architecture to provide accurate predictions.

## Dataset
The dataset contains employee information with various attributes such as age, job satisfaction, income, and more. Key target columns include:
- **Attrition** (Yes/No)
- **Department** (e.g., Sales, HR, R&D)

## Steps to Completion
### Part 1: Preprocessing
- Imported the dataset and examined the data.
- Selected 10 relevant columns for the feature set (`X_df`).
- Encoded the target labels (`y_df`) using `OneHotEncoder`.
- Standardized the feature data using `StandardScaler`.

### Part 2: Create, Compile, and Train the Model
- Created a branched neural network with:
  - Two shared hidden layers.
  - Two output branches:
    - **Department Prediction Branch** — Hidden layer + Softmax output.
    - **Attrition Prediction Branch** — Hidden layer + Softmax output.
- Compiled the model with `Adam` optimizer and `categorical_crossentropy` loss.
- Trained the model and evaluated performance on the test set.

### Part 3: Summary
- Provided insights on the choice of metrics, activation functions, and possible improvements.

## Results
- The model successfully predicts both **Attrition** and **Department** with reasonable accuracy.

## Potential Improvements
- Add dropout layers to reduce overfitting.
- Tune hyperparameters (e.g., learning rate, batch size).
- Balance the dataset if class imbalance exists.

## Repository Structure
├── attrition.ipynb # Main notebook with code implementation ├── README.md # Project overview and instructions ├── data/ # Contains the attrition.csv dataset (if needed)

## Instructions
1. Clone the repository.
2. Upload `attrition.ipynb` to Google Colab.
3. Follow the notebook steps for data preprocessing, model training, and evaluation.
