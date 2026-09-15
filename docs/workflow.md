# Workflow and reproducibility

## Notebook structure

- Brain Tumor Segmentation and Classification
- 1. Data Preparation
- Classifying the Files based on their Labels
- Splitting the Data on the Patient-level
- Extracting the Images and their corresponding masks from the files in .png format
- Saving the Images in .png format across all the classes for both training and validation
- Saving the Masks for the various classes across training and testing groups
- 3. Machine Learning
- Feature extraction
- Feature extractor 1: Grey-Level Co-Occurence Matrix
- Model Training - GLCM
- Model 1 - Logistic Regression
- Model 2: Random Forest Classifier
- Hyperparameter tuning
- Bayesian optimisation - hyperparameter tuning
- RandomForest One-vs-All
- RandomForest Ovr Optimisation
- Dealing with the Class Imbalance
- Resampling
- Model 3 : SVM - GLCM
- Model 4: Extra Trees
- Optimising the Extra Trees

## Required inputs

The notebook describes 3,064 contrast-enhanced T1 images from 233 patients, stored in MATLAB `.mat` files with image, mask, label and patient-ID fields. Obtain the original dataset and place it in the directory structure used by the data-preparation cells; original inputs are not committed.

## Run and interpret

This 359-cell notebook contains exploratory stages and hard-coded Colab/Drive/checkpoint paths. Run a selected stage with its inputs rather than assuming every experimental cell forms one unattended pipeline. Patient identifiers are available in the described data; preserve patient-level separation throughout preprocessing and evaluation. Historical metrics have not been reproduced in this pass.

## Maintenance verification

A stage guide, dependency inventory and links to the related VGG16 project were added; the Colab link now targets the default branch. The notebook was checked as Jupyter format. Any preview in the README comes from existing saved output; the full external-data experiment was not rerun. Package installation and original environment compatibility may need adjustment for the historical code. Data, checkpoints and exported outputs are excluded from Git by default.
