# Machine learning is not about algorithms.

Machine learning is a comprehensive approach to solving problems and individual algorithms are only one piece of the puzzle. The rest of the puzzle is how you apply them the right way.

## What makes machine learning so special?

Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.

For true machine learning, the computer must be able to learn patterns that it's not explicitly programmed to identify.

## Why explore your dataset upfront?

The purpose of exploratory analysis is to "get to know" the dataset. Doing so upfront will make the rest of the project much smoother, in 3 main ways:

1. You’ll gain valuable hints for Data Cleaning (which can make or break your models).
2. You’ll think of ideas for Feature Engineering (which can take your models from good to great).
3. You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

## What is Feature Engineering?

Feature engineering is about creating new input features from your existing ones.

In general, you can think of data cleaning as a process of subtraction and feature engineering as a process of addition.

This is often one of the most valuable tasks a data scientist can do to improve model performance, for 3 big reasons:

1. You can isolate and highlight key information, which helps your algorithms "focus" on what’s important.
2. You can bring in your own domain expertise.
3. Most importantly, once you understand the "vocabulary" of feature engineering, you can bring in other people’s domain expertise!

## Create Interaction Features

The first of these heuristics is checking to see if you can create any interaction features that make sense. These are combinations of two or more features.

By the way, in some contexts, "interaction terms" must be products between two variables. In our context, interaction features can be products, sums, or differences between two features.

A general tip is to look at each pair of features and ask yourself, "could I combine this information in any way that might be even more useful?"

## Combine Sparse Classes

The next heuristic we’ll consider is grouping sparse classes.

Sparse classes (in categorical features) are those that have very few total observations. They can be problematic for certain machine learning algorithms, causing models to be overfit.

* There's no formal rule of how many each class needs.
* It also depends on the size of your dataset and the number of other features you have.
* As a rule of thumb, we recommend combining classes until each one has at least ~50 observations. As with any "rule" of thumb, use this as a guideline (not actually as a rule).
* We might want to group 'Wood Siding', 'Wood Shingle', and 'Wood' into a single class. In fact, let's just label all of them as 'Wood'.
* We'd group 'Concrete Block', 'Stucco', 'Masonry', 'Other', and 'Asbestos shingle' into just 'Other'.

## Add Dummy Variables

Dummy variables are a set of binary (0 or 1) variables that each represent a single class from a categorical feature.

## Remove Unused Features

Finally, remove unused or redundant features from the dataset.

Unused features are those that don’t make sense to pass into our machine learning algorithms. Examples include:

* ID columns
* Features that wouldn't be available at the time of prediction
* Other text descriptions

**Redundant** features would typically be those that have been replaced by other features that you’ve added during feature engineering.

## Why Linear Regression is Flawed

To introduce the reasoning for some of the advanced algorithms, let's start by discussing basic linear regression. Linear regression models are very common

## How to Train ML Models


At last, it’s time to build our models!

It might seem like it took us a while to get here, but professional data scientists actually spend the bulk of their time on the steps leading up to this one:

1. Exploring the data.
2. Cleaning the data.
3. Engineering new features.

Again, that’s because better data beats fancier algorithms.