# Sentiment-Analysis
### Dataset Source : 
https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset?resource=download
<img width="422" alt="image" src="https://github.com/user-attachments/assets/449f8c67-aeca-482a-8db7-a2f8dd91572c">
The dataset file, named sentimentsdataset.csv, encapsulates diverse social media insights. It comprises user-generated content, sentiment labels, timestamps, platform details, trending hashtags, user engagement metrics, and geographical origins. With additional columns for extracted date and time components, this dataset is a valuable resource for sentiment analysis, trend identification, and temporal analysis on social media platforms.
Columns:
● Unnamed: 0: Index column (can be ignored)
● Text: User-generated content (text)
● Sentiment: Target variable indicating the sentiment (Positive, Negative, Neutral)
● Timestamp: Date and time of the post
● User: User who posted the content
● Platform: Social media platform where the content was posted
● Hashtags: Hashtags used in the post
● Retweets: Number of retweets
● Likes: Number of likes
● Country: Geographical origin of the post
● Year, Month, Day, Hour: Extracted date and time components

### Objective :
To train models such that it can classify the text posted over the social media platform is positive, negative or neutral. More importantly further we compare all these models to find out which model will be the most suitable one for our work.
Models Used :
1. SVM
2. Random Forest
3. Gradient Boosting
4. Logistic Regression
5. K-Nearest Neighbors
6. Naive Bayes
7. Decision Tree
8. AdaBoost
9. Extra Trees
10. Bagging Classifier
    
### Flow Of The Work :
Data Collection - Collection Of Dataset.
Data Exploration And Analysis - Exploring the dataset to understand its characteristics, such as the distribution of classes, feature statistics, and potential issues like missing values or outliers. 
Data Preprocessing - Handling missing values and outliers, Normalizing or standardizing numerical features, Encoding categorical variables, Splitting the dataset into training and testing sets.
Feature Engineering - Selecting relevant features, Creating new features if needed, Using techniques like dimensionality reduction if applicable.
Model Selection - Choosing a classification algorithm based on the nature of the problem and dataset, Splitting the training set into a training subset and a validation subset for hyperparameter tuning.
Model Training - Training the chosen model on the training subset, Fine-tuning hyperparameters using the validation subset.
Model Evaluation - Using metrics such as accuracy, precision, recall, F1 score, and ROC-AUC.

The Dataset Encapsulates diverse social media insights. It comprises user-generated content, sentiment labels, timestamps, platform details, trending hashtags, user engagement metrics, and geographical origins. With additional columns for extracted date and time components, the dataset is a valuable resource for sentiment analysis, trend identification, and temporal analysis on social media platforms. It has in total 733 rows and 15 columns. The starting two columns Index and Unnamed can be ignored as they contain serial numbers for each row. Text column contains 707 unique values. It means it has some duplicate values. Sentiment column contains
279 unique values. Platform column contains 4 unique values - Instagram, Facebook, Twitter and others.

<img width="296" alt="image" src="https://github.com/user-attachments/assets/c8b398b0-369a-48a1-8573-dbe05164fd8d">        <img width="256" alt="image" src="https://github.com/user-attachments/assets/a9a23f0f-9738-44a2-b93d-45c965a57cbe">

### Results :

| Model                  | Accuracy  | Precision | Recall   | F1 Score |
|------------------------|-----------|-----------|----------|----------|
| SVM                    | 0.768707  | 0.600907  | 0.768707 | 0.674320 |
| Random Forest          | 0.775510  | 0.682829  | 0.775510 | 0.698429 |
| Gradient Boosting      | 0.741497  | 0.674803  | 0.741497 | 0.704681 |
| Logistic Regression    | 0.761905  | 0.580499  | 0.761905 | 0.658945 |
| K-Nearest Neighbors    | 0.768707  | 0.719955  | 0.768707 | 0.740797 |
| Naive Bayes            | 0.761905  | 0.580499  | 0.761905 | 0.658945 |
| Decision Tree          | 0.768707  | 0.755306  | 0.768707 | 0.752057 |
| AdaBoost               | 0.761905  | 0.586653  | 0.761905 | 0.662679 |
| Extra Trees            | 0.795918  | 0.700247  | 0.795918 | 0.742008 |
| Bagging Classifier     | 0.782313  | 0.700675  | 0.782313 | 0.731350 |

