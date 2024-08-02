# Introduction to ML

<p align="justify">This document contains notes for lecture 1 on Machine Learning for CS229 at Stanford by Dr. Andrew Ng.</p>

<p align="justify">Prerequisites for understanding the notes that follow- </p>

- Big O notation
- Probability
- Random Occurrence
- Eigenvectors (maybe?)

## What is ML?

<p align="justify">Arthur Samuel (1959) - ""Field of study that gives computers the ability to learn without explicitly being programmed"
</p>

<p align="justify">Tom Mitchell (1998) - "Computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P improves with experience E"
</p>

## Supervised Learning

<p align="justify">Example 1 - Housing Price Prediction = dataset of housing size in feet against price. How do I price my hose - Fit a straight line, then predict value using that.
</p>

<p align="justify">Effectively - Supervised Learning = Dataset with inputs x and labels y => goal is to find mapping of x to y
</p>

<p align="justify">This is a Regression problem </p>

<p align="justify">Example 2 - Breast cancer = is it benign or malignant?. 
</p>

<p align="justify">X-axis = size of tumour || Y-axis = malignant or not (0 or 1)
</p>

<p align="justify">This is a classification problem - since y can only take on discrete number of variables and has discrete outputs
</p>

<p align="justify">Most applications of machine learning input X will be multidimensional
</p>

<p align="justify">Multiple features would predict another. Example - tumour size vs patient age = two dimensional vector predicting malignancy.
</p>

<p align="justify">This is a Logistic Regression problem
</p>

<p align="justify">There is an algorithm that uses an infinite number of input features !!!! = Support Vector Machines (SVM) = infinite dimensional vector ??
</p>

<p align="justify">Kernels are a technical method that are the base of learning algorithms that work with an infinitely long list of features = very effective apparently and a form of supervised learning
</p>

<p align="justify">Driving a vehicle using an artificial neural network - during training it watches human drive and 10 times a second it digitizes images in front - collects labelled data = records image + steering direction => uses back-propagation and gradient descent to sharply mimic taught behavior after seeing input x and output y.</p>

## Machine Learning Strategy

<p align="justify">There can be a huge gap in two teams at a company applying the exact same learning algorithm => The most skilled ML practitioners are strategic
</p>

What do you mean by this? = Lot of decisions to make

- collect more data - if more, what type
- try a different learning algorithm
- rent faster GPUs

Good Decisions

- Learning algorithms almost never work the first time = debugging <b>systematically</b>
- Run a profiler and fix existing code instead of trying to make it faster

## Unsupervised Learning

<p align="justify">Dataset with no labels and figure out interesting stuff = <b>k-means clustering</b> </p>

Applications

- Google news reads thousands of articles and groups them together
- Cluster people based on genetic profiles using microarrays
- computing clusters + social network analyses + market segmentation + astronomical data analysis
- unlabelled text data - figure out stuff about linguistic patterns = analogies

<p align="justify">Using unlabelled data and finding interesting things about it
</p>

<p align="justify">Cocktail party problem = if you have a noisy room and record them using microphones = overlapping voices = no labels => how can we have an algorithm separate out people's voices = Independent component analysis to solve this
</p>

<p align="justify">Most of the economic value created by ML is in supervised learning
</p>

<p align="justify">Reinforcement learning = let the helicopter do whatever to find the most optimal way to operate by saying good helicopter lol + good dog bad dog in training = using reward signals</p>