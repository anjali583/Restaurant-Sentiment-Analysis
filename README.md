**Restaurant Review Analysis Using Binomial and Multinomial Naive Bayes Probability Models**


*--------------------------Overview--------------------------*

This project focuses on analyzing restaurant reviews to classify sentiments and understand customer preferences. 
We utilize Binomial and Multinomial Naive Bayes probability models to perform sentiment analysis and evaluate the performance of these models using various feature extraction methods.

*---------------------------Objectives-------------------------*

**1. Data Exploration:** Investigate the dataset to understand its structure and contents.
**2. Data Preprocessing:** Clean and preprocess the review data.
**3. Model Implementation:** Apply Binomial and Multinomial Naive Bayes models with different configurations.
**4. Model Evaluation:** Compare the performance of the models and determine the best approach for sentiment analysis.

*-----------------------------Dataset---------------------------*

The dataset Restaurant_Reviews.tsv consists of:
**1. Review:** Text of customer reviews.
**2. Liked:** Binary label indicating whether the review is positive (1) or negative (0).

*---------------------------Methodology----------------------------*

Data Loading and Preprocessing

![image](https://github.com/user-attachments/assets/675b54a3-83b2-4236-ac7c-80350960c8cb)

*-----------------------Feature Extraction--------------------------*

Four different CountVectorizer configurations were used:

![image](https://github.com/user-attachments/assets/fb3c4c75-8dea-4387-b70a-8fbaaace3d15)

**vectorizer1:** Binary (0/1) representation.
**vectorizer2:** Frequency representation.
**vectorizer3:** Binary representation with stop words removed.
**vectorizer4:** Frequency representation with stop words removed

*----------------------Model Training and Testing-------------------------*

The dataset was split into training and test sets, and both Binomial and Multinomial Naive Bayes models were applied.

![image](https://github.com/user-attachments/assets/0b96e9bd-ef1d-4bc6-b778-4a56fc4248cc)


*-------------------------Model Evaluation----------------------------------*

The accuracy scores for each model were computed to evaluate their performance:

![image](https://github.com/user-attachments/assets/e4f9bf4a-c327-47bd-a845-fa346d48e42b)


*--------------------------Prediction Example------------------------------*

An example review was used to test the Multinomial Naive Bayes model:

![image](https://github.com/user-attachments/assets/24f71437-4d29-4db6-8bf4-13e7d2c826ad)


*---------------------------Results-------------------------------*

**Bernoulli Naive Bayes with Binary Features: Accuracy = 0.712**
**Multinomial Naive Bayes with Frequency Features: Accuracy = 0.788**
**Bernoulli Naive Bayes with Stop Words Removed: Accuracy = 0.780**
**Multinomial Naive Bayes with Stop Words Removed: Accuracy = 0.768**

**The Multinomial Naive Bayes model with frequency features achieved the highest accuracy, making it the most effective model for this task.**

*----------------------------Conclusion-------------------------------*

**The analysis demonstrates that the Multinomial Naive Bayes model with frequency features outperforms other configurations in classifying restaurant reviews. 
It achieved the highest accuracy and accurately predicted the sentiment of a sample review as positive. Thus, for sentiment analysis in this context, the Multinomial Naive Bayes model is preferred.**
