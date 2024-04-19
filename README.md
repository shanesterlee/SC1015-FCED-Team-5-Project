# SC1015 Project: Job listing - Fraudulent or Not?

## Context and Outline
Given the recent surge in global fraud and scams, particularly within job offers, we aim to leverage Natural Language Processing (NLP) techniques to distinguish between legitimate and fake job postings.

Here are the steps taken in our project determining fraudulent jobs:
1. EDA (Exploratory Data Analysis)
2. Data Cleaning
3. NLP techniques
4. Decision Tree 
5. Random Forest
6. Logistic Regression 

## EDA’s Result
- The ratio of Real Jobs to Fake Jobs are: 17014 to 866
- We found that only these details do not have any missing details from the data set:
Job_id, title,telecommuting, has_company_logo, has_questions. Additionally after investigating, these data are in fact not integer data type but a boolean data type
- Among the job listings, we have found that Majority of the job listings come from the USA with more than 10k jobs coming from there.
- Among the Categorical columns we have found that has_company_logo has the highest correlation with fraudulent with a score of -0.26 compared to telecommuting, has_questions with a score of 0.035 and -0.092 respectively.

## Data Cleaning and NLP
- We removed the undesired columns in the data set as they did not provide useful information for the jobs being fraudulent or not. The columns are 'job_id','salary_range' and 'department'.
- For the rest of the categorical columns, we filled up the missing values (na) with “None” to better analyse the dataset.
- For the text data with missing values we filled them up with “  ”.
- We removed location from the columns as well.
- We cleaned the text and titles by removing stop words and Stemming
- Found that Spelling errors are common in Fake job listings. Generated a wordcloud to represent the common words in Titles,Benefits,Company profile, Requirements and overall for both Fake and Real job listings.

## Machine Learning algorithms used
1. Decision Tree
2. Random Forest
3. Logistic Regression

## Results and Conclusion
By utilising 3 different kinds of models, we were able to obtain similar accuracy results on our test data. However, among the 3 models, logistic regression allowed us to obtain a test result with slightly higher accuracy as compared to other 2 which both have accuracy results of 0.98 based on F1 scores. (a weighted harmonic mean of precision and recall)

## Insights gained from this project
- Able to discern unnecessary information from a pool of data
- Learnt about Natural Language Processing (NLP)
- Convert text into weighted numerical representations
- WordCloud to have visual representation of words used
- Understood the models used (Decision Tree, Random Forest, Logistic Regression)
- Concepts about classification report (Precision, Recall, and F1 Score)

## Credit for data
For the data set that we used, it was from Kaggle: https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction

## Contributors
@shanesterlee - NLP, Random Forest, Slides, Video
@kx0224 - Data Cleaning , Logistic Regression, Slides , Video
@kaiiifeng - EDA, Decision Tree, Slides, Video

## References
https://www.ibm.com/topics/natural-language-processing
https://monkeylearn.com/word-clouds/#:~:text=A%20word%20cloud%20
https://www.geeksforgeeks.org/random-forest-classifier-using-scikit-learn/
https://www.geeksforgeeks.org/understanding-logistic-regression/
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html
https://www.statology.org/sklearn-classification-report/
