# Music-sentiment-analysis

## Overview
This project aims to perform sentiment analysis on music reviews using a dataset sourced from Kaggle. The dataset includes two columns: Reviews and Ratings. The primary goal is to classify the sentiment of reviews as positive or negative using a Naive Bayes classifier.

## Dataset
The dataset is sourced from Kaggle and contains the following columns:

- Reviews: Text reviews of music.
- Ratings: Numerical ratings associated with the reviews.

## Pre-processing steps
The following pre-processing steps were applied to the dataset:

1. Filtering Reviews in English: Only reviews written in English were included in the analysis.
2. Text Cleaning:
- Removed stop words.
- Lemmatized words to their root form.
- Eliminated unnecessary punctuations.
3. Label Creation:
- Threshold Approach: Reviews with ratings > 3 were labeled as positive, while ratings < 3 were labeled as negative.
- TextBlob Polarity Approach: Reviews with a polarity > 0 were labeled as positive, while reviews with polarity < 0 were labeled as negative.
4. Under-sampling: The majority class was under-sampled to achieve better classification results.

## Classification Approach
The ML algorithm used was Naive-Bayes for the classification.

## Results
The performance of the Naive Bayes classifier was evaluated using accuracy as the metric.

- TextBlob Dataset: Achieved an accuracy of 59%.
- Threshold Dataset: Achieved an accuracy of 78%.

## Conclusion
The Naive Bayes classifier performed better when using the threshold-based labeling approach, achieving an accuracy of 78% compared to 59% accuracy using TextBlob polarity.

## Future Work
Future improvements could include:

- Experimenting with different machine learning algorithms.
- Enhancing the pre-processing steps, such as using advanced text vectorization techniques.
- Balancing the dataset using different methods to improve classification performance.
