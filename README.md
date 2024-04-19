# SC1015 Project: Job listing - Fraudulent or Not?

## Context and Outline
Given the recent surge in global fraud and scams, particularly within job offers, we aim to leverage Natural Language Processing (NLP) techniques to distinguish between legitimate and fake job postings.

Here are the steps taken in our project determining fraudulent jobs:
- EDA (Exploratory Data Analysis)
- Data Cleaning
- NLP techniques
- Decision Tree 
- Random Forest
- Logistic Regression 

## EDA’s Result
- The ratio of Real Jobs to Fake Jobs are: 17014 to 866
- We found that only these details do not have any missing details from the data set: Job_id, title,telecommuting, has_company_logo, has_questions.
- Among the job listings, we have found that Majority of the job listings come from the USA with more than 10k jobs coming from there.

## Machine Learning algorithms used
1. Decision Tree
2. Random Forest
3. Logistic Regression

## Results and Conclusion
By utilising 3 different kinds of models, we were able to obtain similar accuracy results on our test data. However, among the 3 models, logistic regression allowed us to obtain a test result with slightly higher accuracy  as compared to other 2 which both have accuracy results of 0.98 based on F1 scores. (a weighted harmonic mean of precision and recall)

## Insights gained from this project
- Able to discern unnecessary information from a pool of data
- Learnt about Natural Language Processing (NLP)
- Convert text into weighted numerical representations
- WordCloud to have visual representation of words used
- Understood the models used (Decision Tree, Random Forest, Logistic Regression)
- Concepts about classification report (Precision, Recall, and F1 Score)

## References
