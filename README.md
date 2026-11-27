# Handwritten Symbol Recognition and Multi-Cancer Classification

This repository contains the source code, datasets, and trained models
for handwritten symbol recognition and multi-cancer classification.

## System Requirements

Python 3.11 was used for model training and evaluation. The convolutional
neural network (CNN) and fully connected neural networks (FCNNs) were
implemented using TensorFlow 2.18.0 and Keras 3.8.0. The support vector
machine (SVM) was implemented using LinearSVC from scikit-learn.

The provided notebooks can be executed locally in Jupyter Notebook.

## Installation

Create and activate a Python environment using Anaconda:

```bash
conda create -n dnacode python=3.11 pip
conda activate dnacode
```

Install the required Python packages:

```bash
python -m pip install tensorflow==2.18.0 keras==3.8.0 scikit-learn notebook numpy scipy pandas matplotlib h5py openpyxl opencv-python
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

## Demo and Instructions for Use

### Handwritten Symbol Recognition

Extract the data archive and place both `.npy` files in the same
directory as the corresponding notebook.

Open the notebook and execute the cells sequentially to preprocess
the images, train and evaluate the CNN, and export the trained
convolutional kernel weights.

The model training time was less than one hour in the original run.
The actual runtime may vary depending on the hardware configuration.

### Multi-Cancer Classification

The following notebooks are provided:

- `SVM.ipynb`: Classification of cancer samples and healthy controls.
- `FCNN.ipynb`: Classification of different cancer types.

Both notebooks use the dataset `36RNA_data.xlsx`. Place the dataset
in the same directory as the notebooks and execute the cells
sequentially.
