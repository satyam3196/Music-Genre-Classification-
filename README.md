# Music-Genre-Classification-Using Machine Learning
This repository contains code for classifying music genres as either hip-hop or rock using machine learning.

Requirements
The code requires the following Python packages to be installed:

• pandas

• numpy

• matplotlib

• scikit-learn

Data
The track metadata with genre labels is stored in the file fma-rock-vs-hiphop.csv, and the track metrics with features are stored in the file echonest-metrics.json. The two datasets are merged based on the track ID to create a single dataset with features and labels.

Code Description
The code reads in the preprocessed dataset containing track metadata with genre labels and track metrics. Features and labels are created from this dataset.

The data is then split into training and test sets, which are standardized using StandardScaler. Principal Component Analysis (PCA) is used to reduce the dimensionality of the data.

Two classification models, DecisionTreeClassifier and LogisticRegression, are trained on the data and their classification reports are printed.

To balance the dataset, only the hip-hop tracks and rock tracks are subsetted, and the dataset is combined. The same preprocessing and classification steps are performed on this balanced dataset.

Finally, K-Fold Cross-Validation is used to evaluate the models. The Pipeline function is used to standardize and perform PCA on the data before classification using DecisionTreeClassifier and LogisticRegression. The mean accuracy scores for each model are printed.

Conclusion
The music genre classification problem is a classic example of supervised learning, where we aim to train models to predict a categorical variable based on a set of features. The results of this project demonstrate that machine learning can be used to classify music genres with a high degree of accuracy.
