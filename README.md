# Plagiarism Detection Model, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Problem Statement and Dataset

Plagiarism is widely acknowledged to be a significant and increasing problem for higher education institutions (McCabe 2005; Judge 2008). A wide range of solutions, including several commercial systems, have been proposed to assist the educator in the task of identifying plagiarised work, or even to detect them automatically. Direct comparison of these systems is made difficult by the problems in obtaining genuine examples of plagiarised student work. We describe our initial experiences with constructing a corpus consisting of answers to short questions in which plagiarism has been simulated. This corpus is designed to represent types of plagiarism that are not included in existing corpora and will be a useful addition to the set of resources available for the evaluation of plagiarism detection systems.'

This project is based on Clough, P. and Stevenson, M. (2011) Developing a corpus of plagiarised short answers. Language Resources and Evaluation , 45 (1). pp. 5-24. ISSN 1574-020X. Paper Link is [here](http://eprints.whiterose.ac.uk/42922/2/Clough_42922.pdf)

## Project Overview

In this project, you will be tasked with building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.
* This first notebook is **not** required in your final project submission.

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**

* Upload your train/test feature data to S3.
* Define a binary classification model and a training script.
* Train your model and deploy it using SageMaker.
* Evaluate your deployed classifier.

---
