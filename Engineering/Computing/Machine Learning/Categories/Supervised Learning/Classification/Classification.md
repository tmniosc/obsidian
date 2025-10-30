# Overview

Classification is a type of supervised learning in machine learning, where the goal is to predict a discrete label (category or class) for a given input.

- Input (x): features or data sample (image, text, sound, etc.)
- Output (y): class label(s), e.g.
 - Email → spam or not spam
 - Image → cat, dog, or horse 
 
The model learns to map inputs → labels, and then can classify new unseen samples correctly.

# Types of Classification Problems

| Type                            | Description                                         | Example                               |
| ------------------------------- | --------------------------------------------------- | ------------------------------------- |
| **Binary Classification**       | Two possible classes                                | Positive / Negative, Yes / No         |
| **Multi-class Classification**  | More than two classes, one correct label per sample | Cat / Dog / Bird                      |
| **Multi-label Classification**  | One sample can belong to multiple classes           | An image with both _car_ and _person_ |
| **Imbalanced Classification**   | One class has far fewer samples                     | Fraud detection, rare diseases        |
| **Hierarchical Classification** | Classes organized in a hierarchy                    | Animal → Mammal → Dog / Cat           |
# Common Algorithms

| Category              | Algorithms                            | Key Idea                                          |
| --------------------- | ------------------------------------- | ------------------------------------------------- |
| **Linear Models**     | Logistic Regression                   | Simple, interpretable, efficient for linear data  |
| **Distance-Based**    | K-Nearest Neighbors (KNN)             | Classify based on nearest samples                 |
| **Tree-Based**        | Decision Tree, Random Forest, XGBoost | Powerful, interpretable, non-linear               |
| **Probabilistic**     | Naive Bayes                           | Based on conditional probability and independence |
| **Margin-Based**      | Support Vector Machine (SVM)          | Finds optimal separating hyperplane               |
| **[[Deep Learning]]** | CNNs, RNNs, Transformers              | Automatically learn complex features from data    |
# Links

## Articles
- [What is Classification in Machine Learning? | IBM](https://www.ibm.com/think/topics/classification-machine-learning)
- [Classification  |  Machine Learning  |  Google for Developers](https://developers.google.com/machine-learning/crash-course/classification)
- [Classification in Machine Learning: A Guide for Beginners | DataCamp](https://www.datacamp.com/blog/classification-machine-learning)



