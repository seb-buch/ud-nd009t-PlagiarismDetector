# Plagiarism Project, Machine Learning Deployment

> Note for reviewer: This readme file contains all the important modifications. I hope this will help you to review my code.


This folder contains all the code needed for the project.

## Project Overview

In this project, the purpose is to build a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text.

This project is broken down into three main notebooks:

**Notebook 1: Data Exploration**

Actual notebook file: `1_Data_Exploration.ipynb`

*Tasks done in this notebook:*
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.
* This first notebook is **not** required in your final project submission.

*Modifications or code completions I made:*
* I tweaked the "download data" cell so it avoids downloading data multiple times if it was already done.
* I updated the graphical representation of the notebook using seaborn


**Notebook 2: Feature Engineering**

Actual notebook file: `2_Plagiarism_Feature_Engineering.ipynb`

*Tasks done in this notebook:*
* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

*Modifications or code completions I made:*
* TBD

**Notebook 3: Train and Deploy Your Model in SageMaker**

Actual notebook file: `3_Training_a_Model.ipynb`

*Tasks done in this notebook:*
* Upload your train/test feature data to S3.
* Define a binary classification model and a training script.
* Train your model and deploy it using SageMaker.
* Evaluate your deployed classifier.

*Modifications or code completions I made:*
* TBD