# Plagiarism Project, Machine Learning Deployment

> Note for reviewer: This readme file contains all the important modifications. I hope this will help you to review my code.


This folder contains all the code needed for the project.

## Project Overview

In this project, the purpose is to build a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text.

This project is broken down into three main notebooks, plus an additional one:

**Notebook 1: Data Exploration**

Notebook file: `1_Data_Exploration.ipynb`

*Tasks done in this notebook:*
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.
* This first notebook is **not** required in your final project submission.

*Modifications or code completions I made:*
* I tweaked the "download data" cell so it avoids downloading data multiple times if it was already done.
* I updated the graphical representation of the notebook using seaborn


**Notebook 2: Feature Engineering**

Notebook file: `2_Plagiarism_Feature_Engineering.ipynb`

*Tasks done in this notebook:*
* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

*Modifications or code completions I made:*
* I tweaked the "download data" cell so it avoids downloading data multiple times if it was already done.
* I completed the `numerical_dataframe` function (as requested by the exercise).
* I completed the `calculate_containment` function (as requested by the exercise).
* I answered to `Question 1`.
* I completed the `lcs_norm_word` function (as requested by the exercise).
* I added a cell to display the heatmap for the correlation matrix (Correlated features).
* I added my personal conclusion on the correlation matrix/heatmap (just before `EXERCISE: Create selected train/test data`).
* I completed the `make_csv` function.
* I answered to `Question 2` with a pretty long and detailed answer leading to...
* ... a bonus exercise where I test the 3 options I made in question 2.


**Notebook 3: Train and Deploy Your Model in SageMaker**

Notebook file: `3_Training_a_Model.ipynb`

*Tasks done in this notebook:*
* Upload your train/test feature data to S3.
* Define a binary classification model and a training script.
* Train your model and deploy it using SageMaker.
* Evaluate your deployed classifier.

*Modifications or code completions I made:*
* TBD

**Additional Notebook: Local testing and training**

Notebook file: `3_Training_a_Model_locally.ipynb`

*Tasks done in this notebook:*
* Train and test models on local GPU workstation before running `3_Training_a_Model.ipynb` on AWS SageMaker.