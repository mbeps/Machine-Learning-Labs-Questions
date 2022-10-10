The following exercises involve the iris dataset.

# 1
## Question
Briefly explain the way `np.mean(y_pred == y_test)` is computed. 
It might help to run its part: `y_pred == y_test`.

## Answer
`y_pred == y_test` compares every element `y_pred` list and `y_test` assigning what is true and what is false. 
This creates a list containing boolean values. 
The `mean` function then computes the percentage of true. 

# 2
## Question 

## Answer

# 3
## Question
Check that the dataset that you loaded from file in Section 5 is identical to the one that you loaded using load_iris in Section 1. You may want to use your answer to Exercise 1. If the two data sets are not identical, please explore the difference.

## Answer
The 2 datasets are not the same. `np.array_equal(X, iris['data']` has been used to check if the `iris_data.txt` is the same as the iris dataset which returns false. `np.mean(X == iris['data'])` checks how much of the data from the `iris_text.txt` is the as the iris dataset from scikit learn and it returns 99.5%; this means that most of the data is the same but not identical. 
