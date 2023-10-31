# Movie_Review_Classifier_Updated

## Overview
This project utilizes the `pandas`, `numpy`, and `sklearn` libraries to perform sentiment analysis on movie reviews. The goal is to classify movie reviews as either positive (`pos`) or negative (`neg`) based on the review text.

## Dataset
The dataset is loaded from a tab-separated file `moviereviews2.tsv`. Each row in the dataset contains a label (either `pos` or `neg`) and a corresponding review.


## Data Preprocessing
1. **NaN Values**: The dataset is checked for NaN values and any rows containing NaN values are dropped.
2. **Whitespace Strings**: The dataset is checked for reviews that are just whitespace and any such rows are identified but not removed in this example.

## Model Training
1. **Splitting the Data**: The dataset is split into training and test sets using a 67-33 split ratio.
2. **Vectorization & Classification**: A pipeline is built using `TfidfVectorizer` to vectorize the review texts and `LinearSVC` (Linear Support Vector Classification) for classification.
3. **Model Fitting**: The model is then trained on the training set.

## Model Evaluation
1. **Predictions**: The trained model is used to make predictions on the test set.
2. **Confusion Matrix**: Displays the number of true positive, true negative, false positive, and false negative predictions.
3. **Classification Report**: Provides metrics such as precision, recall, f1-score for both positive and negative classes.
4. **Accuracy**: Displays the overall accuracy of the model on the test set.

## Testing with Custom Inputs
The model can also be tested with custom input strings to check its predictions.

## Dependencies
- pandas
- numpy
- sklearn

## How to Run
1. Ensure you have the necessary libraries installed.
2. Load the dataset from `moviereviews2.tsv`.
3. Follow the steps in the code to preprocess the data, train the model, evaluate its performance, and test with custom inputs.

## Conclusion
The sentiment analysis model demonstrates a high accuracy in classifying movie reviews as either positive or negative. It serves as a useful tool for quickly gauging the sentiment of a given review.

