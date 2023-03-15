# Financial-Fraud-Detection

Dataset: https://www.kaggle.com/datasets/ealaxi/paysim1

# Some properties that dataset already have:

    There are no missing values

    There are just over 6 million observations

    There are 11 variables

    Most transactions involve amounts less than 1 million euros.

    Most observations in the dataset are of valid transactions, so any patterns related to identifying fraud transactions may be hard to see, data is also unbalanced.

    From the sample of observations, there are many instances where what happens to the recipient account (oldbalanceDest, newbalanceDest) does not make sense (e.g. the    very first observation involved a payment of 9839.64 yet, the balance before and after the transaction equals 0.)

# Some of conclusion in EDA:

    The original dataset is imbalanced between Fraud and non-Fraud, most of them are non-fraud.
    
    In a modified dataset with more than 2 million observations, isFlaggedFraud that brings attention to only 16 observations is insignificant.
    
    Name type of Orig and Dest is not necessary 
    
    Only TRANSFER and CASH_OUT transaction approximately have the same number of Fraud
    
# Feature Transformation

A first approach to deal with imbalanced data is to balance it by discarding the majority class before applying an ML algorithm. The disadvantage of undersampling is that a model trained in this way will not perform well on real-world skewed test data since almost all the information was discarded. A better approach might be to oversample the minority class, say by the synthetic minority oversampling technique (SMOTE) contained in the 'imblearn' library. 

# Modeling

Among these algorithms, the extreme gradient-boosted (XGBoost) algorithm used below slightly outperforms others.

![image](https://user-images.githubusercontent.com/83870939/225279073-c82e7e72-d8cb-499f-977f-6484bc02100b.png)

