# EEG-Analysis-Project

## Overview
This task is centered around the analysis of EEG data to classify different cognitive states using advanced deep learning techniques. The data is sourced from the [Mental Arithmetic Tasks Dataset](https://physionet.org/content/eegmat/1.0.0/) available at PhysioNet. The dataset is pre-cleaned and ready for use, allowing you to focus on model implementation and evaluation. Please familiarize yourself with the dataset by reviewing the accompanying research paper [here](https://www.mdpi.com/2306-5729/4/1/14).

## Objectives
You are required to implement and evaluate multiple deep learning models (suggested to implement at least 2 models) using the Python library MNE. Your analysis should be documented in a Jupyter Notebook, which will be submitted via a GitHub repository link.

## Steps to Achieve It

### 1. Load the EEG Data
- Load the EEG data from the provided EDF files using the MNE library.
- Preprocess the data as needed, including filtering and artifact removal.

### 2. Power Spectral Density (PSD) Analysis
#### a. Calculate the Band-Wise PSD for Both States
- Calculate the band-wise PSD for both states: rest (recording EEG dataset before the mental arithmetic task) and task (recording of EEG dataset during the mental arithmetic task).
- Focus on the following frequency bands: Delta (1-4 Hz), Theta (4-8 Hz), Alpha (8-12 Hz), Beta (12-30 Hz), and Gamma (30-100 Hz).

#### b. Compare the PSDs of the Two States
- Compare the PSDs of the rest and task states.
- Summarize your findings.

### 3. Deep Learning Classification
#### a. Extract Relevant Features from the Cleaned Data
- Extract features from the preprocessed EEG data that will be used for classification.

#### b. Implement Binary Classification Using Any Two Different Deep Learning Models
You may choose from the following models:
- EEGNet
- TSCeption
- ViT (Vision Transformer)
- ATCNet
- VAE (Variational Autoencoder)

#### c. Train and Validate the Models
- Train the models using the provided dataset.
- Validate the models using a separate validation set.

#### d. Evaluate the Models
- Evaluate the models using appropriate metrics (accuracy, precision, recall, F1-score).
- Discuss the results and provide insights into the performance of each model.
