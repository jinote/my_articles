Before discussing train_test_split, you should know about Sklearn (or Scikit-learn). 
It is a Python library that offers various features for data processing that can be used for classification, clustering, and model selection.
Model_selection is a method for setting a blueprint to analyze data and then using it to measure new data. Selecting a proper model allows you to generate accurate results when making a prediction.
To do that, you need to train your model by using a specific dataset. Then, you test the model against another dataset.
If you have one dataset, you'll need to split it by using the Sklearn train_test_split function first.


* __What is train_test_split?__

train_test_split is a function in Sklearn model selection for splitting data arrays into two subsets: for training data and for testing data. With this function, you don't need to divide the dataset manually.
By default, Sklearn train_test_split will make random partitions for the two subsets. However, you can also specify a random state for the operation.


* __Parameter__

1. X, y: The first parameter is the dataset you're selecting to use.
2. train_size: This parameter sets the size of the training dataset. There are three options: None, which is the default, Int, which requires the exact number of samples, and float, which ranges from 0.1 to 1.0.
3. test_size: This parameter specifies the size of the testing dataset. The default state suits the training size. It will be set to 0.25 if the training size is set to default.
4. random_state: The default mode performs a random split using np.random. Alternatively, you can add an integer using an exact number.


* __Why use the Sklearn train_test_split function?__

Using the same dataset for both training and testing leaves room for miscalculations, thus increases the chances of inaccurate predictions.
The train_test_split function allows you to break a dataset with ease while pursuing an ideal model. Also, keep in mind that your model should not be overfitting or underfitting.


source:
<https://www.bitdegree.org/learn/train-test-split#:~:text=train_test_split%20function%20first.-,What%20is%20train_test_split%3F,data%20and%20for%20testing%20data.&text=By%20default%2C%20Sklearn%20train_test_split%20will,random%20state%20for%20the%20operation.>
