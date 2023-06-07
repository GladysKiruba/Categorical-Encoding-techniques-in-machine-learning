# Categorical-Encoding-techniques-in-machine-learning
Datasets consists of both numerical and categorical features. Categorical features consist of strings. Machine learning algorithms cannot deal with strings. So these strings have to be converted into numbers by suitable encoding techniques.

**Types of categorical features:**

There are two types of categorical features they are ordinal and nominal.

**i)	Nominal**

Nominal categorical features are the features where the order doesn’t matter. For example gender can be male, female or other and the order is not important

**ii)	Ordinal**

Ordinal categorical features are the features where the order matters. For example, the grades of the students. Here the order is important.

**Types of encoding techniques:**

1)	Label encoding(Nominal encoding)
2)	One Hot encoding
3)	Dummy encoding
4)	Frequency encoding
5)	Binary encoding
6)	Target encoding


**1)	Label encoding (Nominal encoding):**

In Label encoding the order matters, so the grades column will be encoded as 0,1,2,3,4. ‘4’ is the highest grade and ‘0’ is the lowest grade.

**2)	One hot encoder with dummies:**

This encoding method is used for nominal features or where the order doesn’t matter. Here new variables or columns are created for every feature in the column. It is filled with 0’s and 1’s. ‘0’ represents the absence and ‘1’ represents the presence of the variable. One column will be dropped in the dummy encoding, in the last after encoding. 

**3)	One hot encoder using Scikit-learn:**

OneHotEncoder is a built in class in Sklearn . We have to initialize OneHotEncoder object and fit and transform. The data will be replace by arrays of data.

**4)	Binary encoder using Scikit-learn:**

In this method the categorical features are encoded in binary order 000,001,010,011 etc.

**5)	Frequency encoding:**

Frequency encoding technique is used where there are too many variables in the categorical features. If we use one hot encoding the number of columns will be more and it may cause the curse of dimension. In frequency encoding the frequency is calculated by the number of occurrences of the particular variable.

**6)	Target encoding:**

In target encoding the categorical feature is replaced by the average of the target variable. Here for example Banglore city is replaced by the average of the rank corresponding to Banglore city. One disadvantage of using target encoding is overfitting. It is also called as leakage of target variable.


