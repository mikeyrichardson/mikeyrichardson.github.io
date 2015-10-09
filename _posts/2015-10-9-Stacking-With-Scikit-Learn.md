---
layout: post
title: Stacking with Multiple Scikit Learn Models
---
The Liberty Mutual Property Inspection Prediciton was the second competition I participated in on Kaggle. The data contained only anonymous features and I was forced to learn how to stack multiple models together (since I didn't have any hope of engineering significant features based on knowledge of the data). Now, a couple months later, I've learned a bit more about effective stacking and I thought I'd revisit the problem and create an iPython notebook detailing my process.

In order for stacking to be most effective, a variety of different types of models should be used. Sometimes, you might even want to use the same type of model multiple times, but with different parameters. As you train each model, you can evaluate it's accuracy in predicting the training labels. As long as the model does better than random at predicting, it can be useful in the stacking process.

When choosing which models to combine, you also want to look for models that make predictions that are not correlated to the predictions of another model. In other words, three strong models that predict almost the same thing might not be as effective as one strong model and two weaker models that predict very different things. 

The iPython notebook below details the process of stacking models.

[View iPython notebook](https://github.com/mikeyrichardson/stacking_with_sklearn/blob/master/code/StackingDemonstration.ipynb)

 