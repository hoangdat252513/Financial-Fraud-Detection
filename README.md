# Financial-Fraud-Detection

Dataset: https://www.kaggle.com/datasets/ealaxi/paysim1

Some properties that dataset already have:

    There are no missing values

    There are just over 6 million observations

    There are 11 variables

    Most transactions involve amounts less than 1 million euros.

    Most observations in the dataset are of valid transactions, so any patterns related to identifying fraud transactions may be hard to see, data is also unbalanced.

  From the sample of observations, there are many instances where what happens to the recipient account (oldbalanceDest, newbalanceDest) does not make sense (e.g. the    very first observation involved a payment of 9839.64 yet, the balance before and after the transaction equals 0.)
