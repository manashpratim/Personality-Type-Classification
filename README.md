# Personality-Type-Classification
Identifying a person’s personality type based on some text they have written.
# Description
The goal of this project is to identify the personality type (MBTI) of a person based on their online posts. The dataset is available for download at https://www.kaggle.com/datasnaek/mbti-type. 

This dataset contains over 8600 rows of data, on each row is a person’s:
1) Type (This persons 4 letter MBTI code/type)
2) A section of each of the last 50 things they have posted (Each entry separated by "|||" (3 pipe characters))

There are a total of 16 types. This dataset suffers from massive class imbalance problem. The class distributions are as follows:

INFP    1832
INFJ    1470
INTP    1304
INTJ    1091
ENTP     685
ENFP     675
ISTP     337
ISFP     271
ENTJ     231
ISTJ     205
ENFJ     190
ISFJ     166
ESTP      89
ESFP      48
ESFJ      42
ESTJ      39

I have implemented both traditional ML algorithms (Multinomial Naive Bayes, SVM and Random Forests) and Convolutional Neural Network (CNN). The CNN model gives significantly better performance than the traditional ML algorithms. Furthermore, I have tried to tackle the class imbalance problem with the Synthetic Minority Oversampling Technique (SMOTE). This improves the accuracy of CNN by over 1.5% and Cohen Score by over 7%. 
