---
title: "Adaboost"
author: "WeizhouS"
date: "3/18/2019"
output: pdf_document
---
#### Adaboost: adaptive boosting

boosting: combine weak learners to strong learner

ensemble machine learning methods: bagging/boosting/stacking

> bagging: reduce variance, bootstrap aggregation  
  boosting: reduce bias, sequence of weak learners  
  stacking: good

Adaboost: base learner can be any learner accepting weighted sample

- weights for samples  
- weights for classifiers

con: sensitive to noise / outliers, slower than XGBoost

