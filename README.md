# Planet Identifier using CNN (ResNet-inspired)

This project implements a convolutional neural network for classifying images of planets (Earth, Jupiter, Mars, Mercury, Neptune, Saturn, Uranus, Venus). The model is inspired by ResNet-style residual connections and trained using PyTorch.

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

## Setup
```bash
python -m venv .venv
source .venv/Scripts/activate  # Windows
pip install -r requirements.txt


