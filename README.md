# Stochastic Gradient Descent (SGD)-based Issue Report Classifier

This repository contains our code and documentation for participation in The NLBSE'23 Tool Competition. 

## Data Set
We used issue reports data from real open source projects made available by (Kallis et al., [2023] ([https://doi.org/10.1007/978-3-031-21388-5_34](https://github.com/nlbse2023/issue-report-classification)) for **The NLBSE'23 Tool Competition**.

**Training Data: 1275881**

**Testing Data: 142320**

## Steps to run the code 

**Step-1:** Get data 

<code> Training Data: https://tickettagger.blob.core.windows.net/datasets/nlbse23-issue-classification-train.csv.tar.gz</code>

<code> Testing Data: https://tickettagger.blob.core.windows.net/datasets/nlbse23-issue-classification-test.csv.tar.gz </code>

**Step-2:** Install

**sklearn** and **gensim**. On Windows, install using the following command: <code> pip install sklearn </code> and <code> pip install gensim </code> .

**Step-3:** Download

<code> git clone https://github.com/laiqujan/sgd-based-issue-classification.git </code>

<code> cd sgd-based-issue-classification </code>

**Step-4:** Run

Run <code> sgd-based-issue-classification.ipynb </code>. Then execute all cells in the jupyter notebook and check the results.

## Classifier 
We implemented an SGDClassifier with the following parameters:
<code> SGDClassifier(loss='hinge', penalty='l2',alpha=0.000001, random_state=42,max_iter=20, tol=0.001) </code>
Additional hypermeters can be tried; <a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDClassifier.html#sklearn.linear_model.SGDClassifier" target="_blank">visit</a>
 for the full list.
 
## Pre-processing
We followed standard preprocessing steps such as data cleaning and vectorization. We performed data cleaning mainly using Gensim, check the 
<code> def preprocess (text) </code> function. Then we applied TfidfVectorizer.
