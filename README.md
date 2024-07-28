# spam-prediction
# SMS Spam Classifier Project Report
## Introduction
This project aims to develop a spam classifier using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to accurately differentiate between spam and ham (non-spam) messages in the SMS text data.

## Methodology
### 1. Data Acquisition and Preprocessing
* The SMS Spam Collection Dataset from Kaggle was used for this project.


* The dataset contains 5,572 messages with 5 columns.


* Irrelevant columns (Unnamed: 2, Unnamed: 3, Unnamed: 4) were removed.


* Duplicates (403) were dropped from the dataset.


#### 2. Data Exploration and Analysis
* The dataset contained no null values, ensuring data integrity.


* A new column 'message_length' was added to represent the length of each message.


* Statistical summaries revealed insights on message length distribution and other aspects of the data.


* The value counts of target categories ('ham' and 'spam') were calculated.


### 3. Data Visualization

* The distribution of target categories showed that 87.37% were 'ham' messages and 12.63% were 'spam' messages.


* Histograms and box plots revealed the skewness of message length in both categories.


### 4. Data Preprocessing
* Text preprocessing techniques such as lower casing, tokenization, and stemming (using Snowball Stemmer) were applied to the messages.


* Stop words, HTML tags, square brackets, and URLs were removed to clean the text.


### 5. Text Vectorization Using TF-IDF
* TF-IDF vectorization was performed on both the training and test sets to convert text data into numerical form.


* A total of 6012 features were generated using TF-IDF vectorization.



### 6. Train-Test Split
* The data was split into training and test sets in a 80:20 ratio.


* The dimensions of the resulting sets were displayed.
### 7. Model Building and Evaluation


* Nine different classifiers were trained and evaluated using performance metrics.


* Random Forest Classifier demonstrated excellent performance with high accuracy, precision, recall, F1-score, and balanced accuracy.


### 8. Model Evaluation
* Classification reports for both the training and test data were generated, providing insights into precision, recall, and F1-score.


* The confusion matrix in percentage form illustrated the distribution of false positives and false negatives.


### 9. Cross Validation
* Cross-validation was performed to assess model performance and variance.


* The mean accuracy score of the Random Forest Classifier was calculated.
### 10. Model Saving

* The trained Random Forest Classifier model was saved using the joblib library.


## Conclusion
In conclusion, the developed SMS spam classifier successfully differentiates between spam and ham messages with high accuracy and precision. The Random Forest Classifier emerged as the best-performing model, providing consistent results on both training and test data. This project showcases the effectiveness of NLP techniques and machine learning algorithms in tackling text classification tasks.

## Future Work
* Further hyperparameter tuning could be performed to optimize model performance.


* Ensemble methods or deep learning architectures could be explored for potential improvements.


* The model could be integrated into a messaging platform or email client for practical use.
