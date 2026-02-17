# Planet Identifier using CNN (ResNet-inspired)

This project implements a convolutional neural network for classifying images of planets (Earth, Jupiter, Mars, Mercury, Neptune, Saturn, Uranus, Venus). The model is inspired by ResNet-style residual connections and trained using PyTorch.

## Impotant Note: Due to difficulty in training locally to lack of compute this version is specifically made with google collab in mind

## Dataset
The dataset was sourced from Roboflow and contains annotated planetary images split into train, validation, and test sets.  
Due to size constraints, the dataset is not included in this repository.

## Methodology
- Exploratory Data Analysis (EDA) to study class imbalance and visual variability  
- Preprocessing: resizing, normalization, and data augmentation (training only)  
- Model: custom ResNet-inspired CNN  
- Training: class-weighted cross-entropy loss, Adam optimizer  
- Evaluation: accuracy, confusion matrix, precision, recall, F1-score  

## Results
Training curves and confusion matrices are provided in the `results/` directory.

## Setup for running locally
Note : You will need to change the address of datasets accordingly and comment out/delete the cell about mounting google drive to google collab
```bash
python -m venv .venv
source .venv/Scripts/activate  # Windows
pip install -r requirements.txt


