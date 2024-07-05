# Diabetes Classification

A PyTorch based implementation of a binary classification model for predicting the onset of diabetes. The model is trained on the `Pima Indians Diabetes` dataset, which consists of medical records for Pima Indians, and is designed to predict whether a patient will develop diabetes within five years.

## Overview

The notebook guides you through the following steps:

1. Load Data
2. Define the PyTorch Model
3. Define Loss Function and Optimizers
4. Run a Training Loop
5. Evaluate the Model
6. Make Predictions

## Dataset

**Pima Indians Diabetes**:
This dataset contains patient medical record data for Pima Indians and indicates whether they had an onset of diabetes within five years. The problem is framed as a binary classification problem where the onset of diabetes is represented as `1` and no onset as `0`. 

The dataset has 9 columns:

- **Input Variables (X)**:
  1. Number of times pregnant
  2. Plasma glucose concentration at 2 hours in an oral glucose tolerance test
  3. Diastolic blood pressure (mm Hg)
  4. Triceps skin fold thickness (mm)
  5. 2-hour serum insulin (μIU/ml)
  6. Body mass index (weight in kg/(height in m)^2)
  7. Diabetes pedigree function
  8. Age (years)


- **Output Variable (y)**:
  9. Class label (0 or 1)

## Model Architecture

The model is a simple neural network with the following architecture:

- The input layer expects 8 features.
- The first hidden layer has 200 neurons with a `ReLU` activation function.
- The second hidden layer has 100 neurons with a `ReLU` activation function.
- The output layer has 1 neuron with a `sigmoid` activation function.

## Getting Started

1. Clone this repository to your local machine:

```zsh
git clone git@github.com:IsmaelMousa/diabetes-classification.git
```

2. Navigate to the **diabetes-classification** directory:

```zsh
cd diabetes-classification
```

3. Setup virtual environment:

```zsh
python3 -m venv .venv
```

4. Activate the virtual environment:

```zsh
source .venv/bin/activate
```

5. Install the required dependencies:

```zsh
pip install -r requirements.txt
```

6. Run the Jupyter Notebook:
```zsh
jupyter-notebook
```

## Results

The model's performance is evaluated by using the **accuracy** metric, and we got: `88.6%`

## Acknowledgments
The dataset used in this project is available on Kaggle: [Pima Indians Diabetes](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database).
