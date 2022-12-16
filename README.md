# Cisco Competition 8/1 09:00 
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

<img src="./Images/cyber_ariel.png" align="right">
Cisco - Ariel University API Security Detection Challenge 2023

Cisco Competition 8/1 09:00

## Description

The goal of this challenge is to achieve the highest prediction scores while showing advanced data research capabilities in order to map out the right features in the best way fitting your machine learning model of choice. 

You will need to predict and classify malicious and benign API traffic utilizing your knowledge in data exploration and machine learning models. 

In some datasets you will be required to create a model that labels not only the attack but also the attack type.

## Datasets
API security contains four datasets each will be divided to Train (70%), Test (15%), and Validation (15%) while the train-test split will be done inside the code the validation split is gives without labels for later grading.

All the datasets contain HTTP traffic of API requests and responses. 

The datasets are:
1.	Dataset_1: Basic API traffic containing the least number of attacks. 

```
Dataset baseline score:

                   precision    recall  f1-score   support

    Benign          0.95715   0.93922   0.99792       480
    Malware         0.99799   0.94129   0.96881       528
    
    accuracy                            0.96825      1008
    macro avg       0.96860   0.96960   0.96824      1008
    weighted avg    0.97000   0.96825   0.96827      1008

```
2.	Dataset_2
```
Dataset baseline score:

                   precision    recall  f1-score   support

    Benign          0.95715   0.97607   0.96652     30209
    Malware         0.77364   0.ddddd   0.70752      3791

    accuracy                            0.93991     34000
    macro avg       0.86539   0.81394   0.83702     34000
    weighted avg    0.93669   0.93991   0.93764     34000

```
3.	Dataset_3
```
Dataset baseline score:

                   precision    recall  f1-score   support

    Benign          0.95715   0.97607   0.96652     30209
    Malware         0.77364   0.65181   0.70752      3791

    accuracy                            0.93991     34000
    macro avg       0.86539   0.81394   0.83702     34000
    weighted avg    0.93669   0.93991   0.93764     34000
    
```
4.	Dataset_4
```
Dataset baseline score:

                   precision    recall  f1-score   support

    Benign          0.95715   0.97607   0.96652     30209
    Malware         0.77364   0.ddddd   0.70752      3791

    accuracy                            0.93991     34000
    macro avg       0.86539   0.81394   0.83702     34000
    weighted avg    0.93669   0.93991   0.93764     34000
    
```

You will need to prepare four models (one per dataset) from the Train and test sets.
The validation dataset does not contain labels. Once you build your model, please run the validation set and upload the output as described in the submission guide below.

## Baseline Model

Please see the [baseline](./baseling_model.ipynb) model code that contain:
1.	Basic log parsing (you can improve the logic)
2.	Basic feature example of feature extraction (you can improve the logic)
3.	Basic machine learning model (you can create and type of AI/ML model you want)
4.	Output format (this you can’t change the competitions grading code needs this exact format in order to check the result correctly)

Each dataset contains a list of JSON file with this format:
* The log parsing logic reads the JSON and call extract feature function. 
* The features are used to train the mode. You can change each part and adapt it to your own logic.

Once you upload the results to the Google Drive folder the code will analyze your results once a day and return the resulting grades including precision and recall. If your score is in the top 10 your name will appear as a leader in the dataset.

## Scoring
The competition score is based on:
1.	Cisco judges
2.	Competition average top10 ranking
3.	Solution presentation and innovation.

Please see the example [Jupyter code](./baseling_model.ipynb) that will help you start.

## Submission Guide


