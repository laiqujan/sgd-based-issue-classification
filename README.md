# Stochastic Gradient Descent (SGD)-based Issue Report Classifier

This repository provides our code with documentation for participation in The NLBSE'23 Tool Competition. 

## Data Set
We used issue reports from real open source projects data made available by (Kallis et al., [2023] ([https://doi.org/10.1007/978-3-031-21388-5_34](https://github.com/nlbse2023/issue-report-classification)) for **The NLBSE'23 Tool Competition**.

## Required Libraries 
**sklearn** and **gensim**. On Windows, install using the following command: <code> pip install sklearn </code> and <code> pip install gensim </code> 

## Classifier 
We implemented an SGDClassifier with the following parameters:
<code> SGDClassifier(loss='hinge', penalty='l2',alpha=0.000001, random_state=42,max_iter=20, tol=0.001) </code>
Additional hypermeters can be tried; <a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDClassifier.html#sklearn.linear_model.SGDClassifier" target="_blank">visit</a>
 for the full list.
# Pre-processing
