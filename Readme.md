# Music Genre Classification

In the dynamic era of music, it is really challenging to categorize music based on their genre. In this project, we tried to use two different machine learning approach for music classification. We have used (“GTZAN Dataset - Music Genre Classification”) genre collection dataset as it had a large selection of genres, covering hip-hop, jazz, rock and many others which would create a good mix for classification.

# Data Exploration

After downloading the whole zipped file, please make sure you have the dataset and code in the same folder.The original file is a ipynb file, you can use Jupyter notebook, google collab to run this code. Some data exploratory codes are commented out, please remove the comment function to look at the output (Types of attributes, no of attributes,missing attributes etc)



# K- Nearest Neighbor

Instead of performing explicit generalization, it compares new problem instances with instances seen in training, which have been stored in memory.Because computation is postponed until a new instance is observed, these algorithms are sometimes referred to as lazy. Compare to Model-based Learning we don't need to store the data after training. It requires three things Requires three things 1)The set of labeled records 2)Distance Metric to compute distance between records 3)The value of k, the number of nearest neighbors to retrieve.

For KNN, we will be splitting our data Train-test: 70%-30% (we have small dataset around ≈1000) We will try to find the best k value using cross validation (using both 5 and 10 folds). We have scaled data to preventdistance measures from being dominated by one of the attributes.

# KNN with optimum K

New KNN model was created with optimum K value.

# Accuracy vs K_value

This section shows how training and test dataset accuracy will change with respect to different K values. We have selected K range from 1 to 40 for this section.

# Classification Report for KNN

In this section, you will be able to create a classification report containing precision, recall, F score and accuracy.

# Support Vector Machine (SVM)

Support vector machines (SVMs) are supervised learning models with associated learning algorithms that analyze data for classification and regression analysis.In addition to performing linear classification, SVMs can efficiently perform a non-linear classification using what is called the kernel trick, implicitly mapping their inputs into high-dimensional feature spaces. 

We will be splitting our data Train-test: 70%-30% (we have small dataset around ≈1000).For our project we have used RBF kernel as our dataset was non linearly separable. We have also cross validated for tuning C and gamma parameters. For cross validation we have used 10 folds. For C parameter we took data range [0.01, 0.1, 1, 10, 100, 1000] and for gamma [1e-4, 1e-3, 1e-2, 1e-1, 1, 10].

# SVM with optimized parameters

New KNN model was created with optimum K value.

# Accuracy vs C

This section shows how training and test dataset accuracy will change with respect to different C values. We have selected C parameter range [0.01, 0.1, 1, 10, 100, 1000].

# Accuracy vs Gamma

This section shows how training and test dataset accuracy will change with respect to different gamma. We have selected gamma parameter [1e-4, 1e-3, 1e-2, 1e-1, 1, 10].

# Classification Report For SVM

In this section, you will be able to create a classification report containing precision, recall, F score and accuracy.
