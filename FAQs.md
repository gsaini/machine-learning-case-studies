# Frequently Asked Questions — Machine Learning

## Table of contents

1. [What is Machine Learning?](#what-is-machine-learning)
2. [What is Supervised Learning?](#what-is-supervised-learning)
3. [What is a Model?](#what-is-a-model)
4. [What do you mean by an algorithm?](#what-do-you-mean-by-an-algorithm)
5. [Why do we split data into train and test sets?](#why-do-we-split-data-into-train-and-test-sets)
6. [When and how do you bring in test data?](#when-and-how-do-you-bring-in-test-data)
7. [Why do we need to study the mathematics behind the algorithms when we can implement the algorithms using simple codes?](#why-do-we-need-to-study-the-mathematics-behind-the-algorithms-when-we-can-implement-the-algorithms-using-simple-codes)

---

## What is Machine Learning?

Machine learning (ML) is the branch of computer science that enables systems to learn from data and make predictions or decisions without being explicitly programmed for the task.

Key points:

- ML learns patterns from existing data (the training data).
- The learned model performs a task (for example: predicting outcomes).
- Performance is measured with appropriate metrics (accuracy, RMSE, AUC, etc.).

Example

> Playing chess: the experience of playing many games is the "learning" part. The task is playing a game and the performance indicator is the probability (or likelihood) that the program will win the next game.

ML problems are commonly classified into broad categories such as supervised learning and unsupervised learning.

## What is Supervised Learning?

Supervised learning is a type of ML where the target (label) values are known during training. The model learns a mapping from inputs (features) to the target.

Two main types:

- Regression — target is continuous (e.g., house prices).
- Classification — target is categorical/discrete (e.g., disease: yes/no).

Examples

- Regression: Predicting house price from features like area, number of rooms, presence of a pool, etc.
- Classification: Predicting whether a person will be diabetic based on measurements such as blood pressure, glucose level, insulin, etc.

## What is a Model?

A machine learning model is a mathematical or statistical representation of a real-world process. Given training data and an algorithm, the model encodes the relationship between inputs and outputs.

Example

- A house price model takes features such as area and number of rooms and outputs a predicted price.

## What do you mean by an algorithm?

An ML algorithm is a procedure that takes a training dataset and fits a model by estimating relationships between independent (input) variables and the dependent (target) variable.

The algorithm searches for a parameterized function (or structure) that best explains the training data according to some loss function.

## Why do we split data into train and test sets?

Splitting data helps estimate how well a model will perform on unseen data. If a model only performs well on the data it was trained on, it may have overfit and will not generalize.

Typical split

- Training set: used to fit the model.
- Test set (or hold-out set): used to evaluate the model's generalization performance.

Good test-set performance suggests the model may perform well on new data, assuming:

- Data samples were drawn independently and at random.
- The test set is large and representative enough of the target population.

## When and how do you bring in test data?

Initially, the dataset that is provided for analysis is split into train and test sets. The test set should be such that it is representative of the population on which the model is going to make predictions.


## Why do we need to study the mathematics behind the algorithms when we can implement the algorithms using simple codes?

The supervised learning course is the first step in the introduction to modeling in your AI-ML journey. The mathematical content in the videos is covered to give a perception of how algorithms work at the backend and the hands-on videos are covered to demonstrate the implementation of the algorithms. The mathematical intuition behind the algorithms is helpful when you need to improve the performance of your model, in such situations knowing about hyperparameters and what parameters are affecting your model will give you an advantage. A deeper understanding of the algorithms increases the interpretability power of your model.
