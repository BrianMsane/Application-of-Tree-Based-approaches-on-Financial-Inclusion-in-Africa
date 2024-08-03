# Application-of-Tree-Based-approaches-on-Financial-Inclusion-in-Africa


## Introduction
Financial inclusion (FI) is the ability of business entrepreneurs and individuals to access financial products and services with the view to satisfy the needs of their clients or customers. 
In Africa, majority of the people are financially excluded as gathered from the dataset through the graph on the right. 

This may be silently due to the educational level, job type and access to technology,  amongst other attributes. 
The question that led to the research is “Can tree-based algorithms be used for financial inclusion?” so we based our models on almost all the algorithms that are stemmed from the decision trees. 

## Data
The data were collected from https://zindi.africa/competitions/financial-inclusion-in-africa/data and contains 23524 records of participants from Kenya, Rwanda, Tanzania and Uganda which were collected from 2016 through 2018.
Each record has 12 features and the target variable.
The dataset was imbalanced with 86% having bank accounts and 14% does not have the bank account.

## Methodology
- In this study, we carried out the experiments using Decision Trees - DT, Random Forest Classifier - RFC, Gradient Boosting - GB, AdaBoost – Adaptive Boosting, Bagging Classifier - BC, algorithms by calibrating their parameter on resampled and raw imbalanced data – as proved by the Exploratory Data Analysis. 
- Resampling the data was performed by Synthetic Minority Oversampling Technique (SMOTE) which uses the k-nearest neighbour algorithm to create synthetic points. 
- Feature engineering, as known to enhance the predictive power of the model/algorithm, was used and concepts were discretization of numeric features, encoding qualitative features, feature selection - using recursive feature selection, standardization and hyperparameter tuning to harness the model algorithm and find optimal model. 
- A classification problem can either be a single-class or a multi-class and in this study we used the single-label approach through employing binary classification. 
According to Bej, Saptarshi [1], the balanced accuracy is the best metric used to measure and evaluate the performance of high imbalanced class datasets. Other metrics used were the accuracy, balanced accuracy and mean squared error. 
- Random Forest Classifier creates a bootstrapped dataset from which decision trees are made considering only the subset features that ate on that bootstrap. This is done as per the number of trees parameter and then the final decision we consider the majority class, that can be seen on the image on the left.
Done avoid the overfitting nature of decision tree.


## Results
The results showed that DT, AdaBoost, and Bagging classifiers are underperforming in terms of balanced accuracy but their accuracies are almost the mean.
Decision trees are algorithms that perform poorly with data that has noise. 
AdaBoost trains weak learner sequentially and the data points that are incorrectly classified are given more weight and the next weak learner give it more attention and this leads to them performing badly on noisy data.
When the classifiers are trained in parallel with BC, the voting tends to be biased –only going to the majority class.
The results shows that when the noise has been handled with capping the outliers before the modelling part, all the models perform better but the RFC outperformed all the others.  Apparently they are all sensitive to noise.
The Table below gives a brief overview on the results when all the techniques that are specified on the methodology are implemented.


