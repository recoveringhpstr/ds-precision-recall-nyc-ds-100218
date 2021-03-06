
# Classification Errors

Now that we've started discussing classification, it's time to examine comparing our models to each other and choosing models of best fit. Previously in regression, we've been predicting values so it made sense to discuss error as a distance of how far off our estimates were. In classifying a binary variable however, we are either correct or incorrect. As a result, we tend to deconstruct this as how many false positives versus false negatives we come across.  
In particular, we examine a few different specific measurements when evaluating the performance of a classification algorithm.  
  
$Precision = \frac{\text{Number of True Positives}}{\text{Number of Actual Total Positives}}$    
  

$Recall = \frac{\text{Number of True Positives}}{\text{Number of Predicted Positives}}$  
  
$Accuracy = \frac{\text{Number of True Positives + True Negatives}}{\text{Total Observations}}$

![](./images/Precisionrecall.png)

At times, we may wish to tune a classification algorithm to optimize against precison or recall rather then overall accuracy. For example, imagine the scenario of predicting whether or not a patient is at risk for cancer and should be brought in for additional testing. In cases such as this, we often may want to cast a slightly wider net, and it is much preferable to optimize for precision, the number of cancer positive cases, then it is to optimize recall, the percentage of our predicted cancer-risk patients who are indeed positive.

## 1. Split the data into train and test sets


```python
import pandas as pd
df = pd.read_csv()

```


```python
#Your code here
```

## 2. Create a standard logistic regression model


```python
#Your code here
```

## 3. Write a function to calculate the precision


```python
def precision(y_hat, y):
    #Your code here
```

## 4. Write a function to calculate the recall


```python
def recall(y_hat, y):
    #Your code here
```

## 5. Write a function to calculate the accuracy


```python
def accuracy(y_hat, y):
    #Your code here
```

## 6. Calculate the precision, recall and accuracy of your classifier

Do this for both the train and the test set.


```python
#Your code here
```

## 7. Comparing Precision Recall and Accuracy of Test vs Train Sets


Plot the precision, recall and accuracy for test and train splits using different train set sizes. What do you notice?


```python
importimport  matplotlib.pyplotmatplot  as plt
%matplotlib inline
```


```python
training_Precision = []
testing_Precision = []
training_Recall = []
testing_Recall = []
training_Accuracy = []
testing_Accuracy = []

for i in range(10,95):
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size= None) #replace the "None" here
    logreg = LogisticRegression(fit_intercept = False, C = 1e12)
    model_log = None
    y_hat_test = None
    y_hat_train = None

# 6 lines of code here
```

Create 3 scatter plots looking at the test and train precision in the first one, test and train recall in the second one, and testing and training accuracy in the third one.


```python
# code for test and train precision
```


```python
# code for test and train recall
```


```python
# code for test and train accuracy
```
