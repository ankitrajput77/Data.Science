- Naive Bayes is a simple but effective probabilistic machine learning algorithm used for classification and text analysis tasks, such as spam detection and sentiment analysis. It's based on Bayes' theorem and is considered "naive" because it makes a strong assumption that all features (attributes or variables) are independent of each other, which is often an oversimplification but still works well in many practical scenarios.

## Here's a brief explanation of how Naive Bayes works:

1. Bayes' Theorem: Naive Bayes is built on Bayes' theorem, which calculates the probability of an event based on prior knowledge of conditions that might be related to the event.

2. Feature Independence Assumption: Naive Bayes assumes that all features used for classification are independent of each other. This means that the presence or absence of one feature doesn't affect the presence or absence of another feature. This simplifying assumption is where the "naive" in Naive Bayes comes from.

3. Training: To build a Naive Bayes classifier, you start by training it on a labeled dataset. It calculates the probabilities of each feature occurring with each class in the training data.

4. Classification: When you want to classify a new data point, Naive Bayes calculates the probability of it belonging to each class based on the probabilities it learned during training.

5. Decision Rule: Naive Bayes uses a decision rule known as the Maximum A Posteriori (MAP) rule to select the class with the highest probability as the predicted class for the new data point.
   

- The main advantage of Naive Bayes is its simplicity and efficiency, making it especially useful for tasks with a large number of features and relatively small datasets. However, its "naive" assumption of feature independence may not hold in some real-world situations, leading to suboptimal performance compared to more complex algorithms.

- Now, before moving to the formula for Naive Bayes, it is important to know about Bayes’ theorem.

# Bayes’ Theorem

- Bayes’ Theorem finds the probability of an event occurring given the probability of another event that has already occurred. Bayes’ theorem is stated mathematically as the following equation:
  ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/5be07f76-d3a2-4d1d-abd0-98a029442532)
- where A and B are events and P(B) ≠ 0.

- Basically, we are trying to find probability of event A, given the event B is true. Event B is also termed as evidence.
- P(A) is the priori of A (the prior probability, i.e. Probability of event before evidence is seen). The evidence is an attribute value of an unknown instance(here, it is event B).
- P(A|B) is a posteriori probability of B, i.e. probability of event after evidence is seen.
Now, with regards to our dataset, we can apply Bayes’ theorem in following way:
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/6f08579f-ec87-4327-9a96-18f57a77cac0)
where, y is class variable and X is a dependent feature vector (of size n) where:
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/58ba370a-2f36-4bae-b0b6-0ff5da50eab6)
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/a07b4b03-4e11-4cc2-87f4-91f073dbdc72)
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/70545381-a226-4cc6-8e69-59239737648e)
Now, as the denominator remains constant for a given input, we can remove that term:
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/6cc7b63c-7787-4c7f-bd3f-459def6615e2)

Now, we need to create a classifier model. For this, we find the probability of given set of inputs for all possible values of the class variable y and pick up the output with maximum probability. This can be expressed mathematically as:
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/1d4f9b32-1939-40aa-ae08-bbbb1ed89aad)


- so, finally, we are left with the task of calculating P(y) and P(xi | y).

- Please note that P(y) is also called class probability and P(xi | y) is called conditional probability.

- The different naive Bayes classifiers differ mainly by the assumptions they make regarding the distribution of P(xi | y).

- Let us try to apply the above formula manually on our weather dataset. For this, we need to do some precomputations on our dataset.

- We need to find P(xi | yj) for each xi in X and yj in y. All these calculations have been demonstrated in the tables below:
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/cd14f7d4-5189-4ba5-ab89-35ad87280550)
- So, in the figure above, we have calculated P(xi | yj) for each xi in X and yj in y manually in the tables 1-4. For example, probability of playing golf given that the temperature is cool, i.e P(temp. = cool | play golf = Yes) = 3/9.

- Also, we need to find class probabilities (P(y)) which has been calculated in the table 5. For example, P(play golf = Yes) = 9/14.

- So now, we are done with our pre-computations and the classifier is ready!

- Let us test it on a new set of features (let us call it today):
- today = (Sunny, Hot, Normal, False)
- ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/34f6e830-9785-4198-bcd7-79b622ec9d4a)
- ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/01d26ec3-9274-43f7-a860-e15862a1b62f)
- ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/279b930d-3b8b-4c21-8548-b13b7031bdd4)
- ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/2a100f41-d26a-43c0-8aef-9dbe5943adbc)
- ![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/13c520de-c0d5-473d-b7ba-966262c18f8d)
- 







