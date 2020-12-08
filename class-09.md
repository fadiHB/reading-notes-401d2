
# Enriching Your Python Classes With Dunder (Magic, Special) Methods

## What Are Dunder Methods?

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__.

## Special Methods and the Python Data Model

This elegant design is known as the Python data model and lets developers tap into rich language features like sequences, iteration, operator overloading, attribute access, etc.

## Enriching a Simple Account Class
Object Initialization: __init__
Object Representation: __str__, __repr__
Iteration: __len__, __getitem__, __reversed__
Operator Overloading for Comparing Accounts: __eq__, __lt__
Operator Overloading for Merging Accounts: __add__
Callable Python Objects: __call__
Context Manager Support and the With Statement: __enter__, __exit__

## Basic Statistics in Python

### What is probability?

At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?” An event is some outcome of interest. To calculate the chance of an event happening, we also need to consider all the other events that can occur. The quintessential representation of probability is the humble coin toss. In a coin toss the only events that can happen are:

* Flipping a heads
* Flipping a tails

These two events form the sample space, the set of all possible events that can happen. To calculate the probability of an event occurring, we count how many times are event of interest can occur (say flipping heads) and dividing it by the sample space. Thus, probability will tell us that an ideal coin will have a 1-in-2 chance of being heads or tails. By looking at the events that can occur, probability gives us a framework for making predictions about how often events will happen. However, even though it seems obvious, if we actually try to toss some coins, we’re likely to get an abnormally high or low counts of heads every once in a while. If we don’t want to make the assumption that the coin is fair, what can we do? We can gather data! We can use statistics to calculate probabilities based on observations from the real world and check how it compares to the ideal.

### Revisiting the normal

The normal distribution is significant to probability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule.