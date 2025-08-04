# Transfer Learning for Neural Decoding – Neuromatch 2023

This project demonstrates how transfer learning can be applied to decode neural activity from fMRI responses using features extracted from pretrained deep neural networks. The work is based on the Neuromatch Academy 2023 curriculum.

## 🧠 Project Description

The notebook walks through the process of:
- Loading and preprocessing visual stimuli and fMRI data
- Extracting image features using pretrained CNNs (e.g., ResNet18)
- Training linear encoding models to map image features to brain responses
- Evaluating model performance using correlation metrics
- Exploring generalization through transfer learning across subjects or regions

The goal is to investigate how well representations from artificial neural networks align with those in the human brain, and how transferable those representations are across different conditions.

## 📂 Data

The dataset is a curated subset of the Natural Scenes Dataset (NSD), containing:
- Natural image stimuli
- Voxel-wise fMRI responses from visual brain areas

All data is preprocessed and formatted for easy use within the notebook.

## ⚙️ Dependencies

To run the notebook locally, install the following packages:

```bash
pip install torch torchvision numpy matplotlib scikit-learn h5py
