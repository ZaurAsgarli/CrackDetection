Crack Detection using U-Net
Overview

This project implements a convolutional neural network (U-Net) for automatic crack detection in concrete structures. The model is trained and evaluated on an image dataset containing concrete surfaces with and without cracks, along with corresponding segmentation masks. The goal is to detect and localize cracks in the images.

Repository Structure
CrackDetection/
├── CrackDetection.ipynb     # Main notebook (training and evaluation)
├── requirements.txt         # Python dependencies
├── data/                    # Dataset (already included in this repo)
│   ├── Train/
│   │   ├── images/
│   │   └── masks/
│   └── Test/
│       ├── images/
│       └── masks/
└── README.md

Dataset

This project uses the Concrete Crack Dataset
 created by Mert Kerem Tas.
A copy of the dataset is included in this repository under the data/ folder for convenience.
If you wish to download the dataset directly from Kaggle, please refer to the official dataset page.

Dataset structure:

data/
├── Train/
│   ├── images/
│   └── masks/
└── Test/
    ├── images/
    └── masks/

Installation

Clone the repository:

git clone https://github.com/ZaurAsgarli/CrackDetection.git
cd CrackDetection


Create and activate a virtual environment (recommended):

python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows


Install dependencies:

pip install -r requirements.txt

Usage

Ensure that the data/ folder is present in the repository (already included here).

Open the notebook:

jupyter notebook CrackDetection.ipynb


Run all cells to train and evaluate the model.
The notebook includes data preprocessing, model training, evaluation, and visualization of predictions.

Requirements

The main libraries used in this project are:

TensorFlow

NumPy

Matplotlib

All dependencies can be installed from requirements.txt.

Results

The U-Net model is trained with Binary Cross Entropy and Dice loss. The notebook provides visualization of:

Input images

Ground truth segmentation masks

Predicted segmentation masks

These results demonstrate the model’s ability to detect cracks in concrete images.
