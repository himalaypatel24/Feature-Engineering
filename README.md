# Feature-Engineering:
#https://www.kaggle.com/aditya1702/mercedes-benz-data-exploration/data

Here we are working with mercedesbenz data which has around 40 categorical columns and each categorical column has more than 40 categories.

## In this project we will see a technique to handle categorical variables that have high cardinality.
###  Here we use One Hot Encoding - variables with many categories:

What is One Hot Encoding?
One Hot Encoding is a method that allows us to use groups of bits to represent categorical values.
Basically extra columns are created for each categorical value and a 1 is placed in the column of the corresponding category.
If we use basic pandas get_dummies function we  can observe that from with just 5 categorical features we are getting 111 features with the help of one hot encoding.which is not advisable its called as dimensional curse.
So,
To Come over such problem we can take refernce from 
#### KDD Cup Orange Challenge

What can we do instead?

http://proceedings.mlr.press/v7/niculescu09/niculescu09.pdf
In the winning solution of the KDD 2009 cup: "Winning the KDD Cup Orange Challenge with Ensemble 

###### The Team suggested using 10 most frequent labels convert them into dummy variables using one hot encoding:
### So here I have shown how to do it in python.
