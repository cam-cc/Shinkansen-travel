# Shinkansen Bullet train user experience

Predicting Passenger Satisfaction on Shinkansen Bullet Train
# Description

This aim of this project was to predict whether a passenger was satisfied or not considering their overall experience of traveling on the Shinkansen Bullet Train. The problem consists of two separate datasets: Travel data and Survey data, which have been split into two groups and provided in the Dataset folder. The training set can be used to build the machine-learning model, and the testing set should be used to see how well the model performs on unseen data.

# Dataset

The dataset consists of Travel data and Survey data. Travel data has information related to passengers and attributes related to the Shinkansen train, in which they traveled. The survey data is aggregated data of surveys indicating the post-service experience. The data has been split into two groups and provided in the Dataset folder. The folder contains both train and test data separately. The target variable is Overall_Experience, where 1 represents ‘<b>satisfied</b>’, and 0 represents ‘<b>not satisfied</b>’.

The datasets were subjected to necessary data cleaning/validation steps as required.

# Output File Format

The output file format is a CSV file with exactly 35,602 entries plus a header row. The file has two columns: ID and Overall_Experience, which contains 0 & 1 values, where 1 represents ‘Satisfied’, and 0 represents ‘Not Satisfied’.

# Evaluation metric

The evaluation metric is the accuracy score, which is the percentage of predictions made by the model that turned out to be correct. The best possible accuracy is 100% (or 1), and the worst possible accuracy is 0%.

# Results

The models AdaBoost with default parameters (ada1) and AdaBoost with a learning rate of 0.1 (ada2) were both able to achieve an accuracy of <b>95%</b> on the test set.

# Dependencies

    Python 3.x
    pandas
    scikit-learn
    numpy
    scipy
