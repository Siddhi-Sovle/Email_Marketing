# Email Marketing Campaign


colab link : https://colab.research.google.com/drive/1WcgQZtayEqI3veXrXvUI8oc39kfnzn8H?usp=sharing

Answering the questions given in the assigment:



1.   What percentage of users opened the email and what percentage clicked on the link within the email?

  **Ans ->** Originally, it was open-rate=10.35%, click-through rate=2.12% .

2.   Based on all the information you have about the emails that were sent, can you build a model to optimize in future how to send emails to maximize the probability of users clicking on the link inside the email?

  **Ans ->** Yes, firstly, since the target variable "clicked" was imbalanced, I had done oversampling, but making the target ratio as 0.9, which means the number of clicked (1) users to be 90% of the number of not clicked (0) users. This was done so that the model takes in real-world scenarios. After applying feature engineering techniques, I had gine for LightBGM as the main model.
  As, LightBGM was able to:

  Precision (for class 1 = clicked): 0.93, i.e 93% of the time, when the model predicts a user will click, it’s correct.

  Recall (for class 1): 0.99, i.e The model is catching nearly all the users who actually clicked—only missing about 1%.

  F1-score (for class 1): 0.96, i.e Strong balance between precision and recall.

  Accuracy: 96%, i.e since imbalanced data is dealt well, that's why got 96% accuracy.

