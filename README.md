# First-Project

Spam or Ham?

The goal of this experiment was to see if I could train a model to recognize spam emails.

Spam: Spam messages

Ham: Normal messages

Overview:

This experiment utilizes a Naive Bayes model to classify text.

    I started by just testing the model's ability to predict data from the dataset, testing different
max features counts. The most accurate model was using a max feature count of 1000. So I took the model using 1000 max features and compared it to a dataset with only 5 spam or ham messages. This resulted in a low accuracy of 33% so I got a bigger dataset. The next dataset contain 100 messages, using the same model I got an accuracy score of 70%. 70% is ok but I wanted a more precise model, so I looked into hyperparameters tuning. First I created a dictionary called param_grid, which stored alpha and fit_prior. The alpha value helps the model with unseen data which is important because the original data set could be outdated and not have enough data to predict more recent emails. fit_prior learns the probability of a spam or ham email from the training dataset but it should not make a difference because the training data set should contain half spam and half ham emails. Then I use the best model and use it to predict the new data set with 100 messages. The outcome was a 76% accuracy which was a 6% improvement, this is a decent improvement and a change I would make is to increase the size of both the training and outside data set to see if that would give me a more accurate model. I would also like to change the percentages of spam or ham emails so fit_prior would be more effective.

Summary:

    My Naive Bayes model used to classify spam and ham emails performs well when only working with data 
within the original dataset. When new data gets introduce, the model will have a lower accuracy, although not struggling will need some work or more training.