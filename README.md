
## PROJECT TITLE

EEG-Based Neural Markers of Internet Addiction: A Frequency Analysis Using High-Density EEG

## OVERVIEW

This thesis investigates neural markers of Internet Addiction (IA) by analyzing EEG frequency bands from LEMON and functional connenctome phenotyping datasets. Using resting-state high-density EEG data combined with Internet Addiction Test (IAT) scores, machine learning models are trained to classify individuals or non-addicted. Data augmentation techniques were applied to enhance the training data and improve classification robustness.

## DATASETS

LEMON Dataset: resting-state EEG data collected from 216 healthy participants using a 62-channel EEG system (https://fcon_1000.projects.nitrc.org/indi/retro/MPI_LEMON.html)
Functional Connectome Phenotyping Dataset: provides behavioral assessments, including IAT scores (https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/VMJ6NV)

## METHODOLOGY

Data preparation: merged two datasets and filtered for valid IAT scores
Data augmentation: applied time-domain augmentations on EEG signals including Gaussian noise addition and time rehersal to increase sample size and improve classification robustness
Feature extraction: computed PSD for standard EEG frequency bands 
Machine Learning: trained logistic regression and SVM on global frequency features
Analysis: evaluated model performance using accuracy, precision, recall, and F1-score

## USAGE
- Python 3x
- Libraries: pandas, numpy, mne, scipy, scikit-learn, matplotlib, seaborn
- access to LEMON and functional connectome phenotyping datasets (path must be changed in the script)
Notebooks are structured for Google Colab usage and mounted Google Drive paths for data loading
