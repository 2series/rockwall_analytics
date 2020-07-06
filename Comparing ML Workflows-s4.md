# ML Workflow
## June 6, 2020
## About RIHAD VARIAWA
> As a Data Scientist and former head of global fintech research at Malastare.ai, I find fulfillment tacking challenges to solve complex problems using data

*This blog summaries 2 distinct workflows for approaching ML (machine learning) tasks, followed by a distilled 3rd. Do they differ considerably (or at all) from each other, or from other such processes available?*

![](https://media.giphy.com/media/xUySTOigOUHucl3rfW/giphy.gif)

**Is it worth comparing approaches to the ML process?
Are there any fundamental differences between such workflows?**

Though classical approaches to ML tasks exist, and have existed for some time, it's worth taking consult from new and different perspectives for a variety of reasons:

> *Have I missed something? Are there new approaches which had not previously been considered? Should I change my perspective on how I approach ML?*

The 2 most recent resources I've come across outlining workflows for approaching the process of ML are Yufeng Guo's [The 7 Steps of Machine Learning](https://towardsdatascience.com/the-7-steps-of-machine-learning-2877d7e5548e) and section 4.5 of Francois Chollet's Deep Learning with Python. Are either of these any different than how you already process a ML task?

What follows are outlines of these 2 supervised ML approaches, a brief comparison, and an attempt to reconcile the 2 into a 3rd workflow highlighting the most important areas of the supervised machine learning process

**7 Steps of Machine Learning**

I actually came across Guo's article by way of first watching a video of his on YouTube, which came recommended after an afternoon of going down the Google I/O 2018 video playlist rabbit hole. The post is the same content as the video, and so if interested one of the two resources will suffice

1 - Data Collection

+ The quantity & quality of your data dictate how accurate our model is
+ The outcome of this step is generally a representation of data (Guo simplifies to specifying a table) which we will use for training
+ Using pre-collected data, by way of datasets from Kaggle, UCI, etc., still fits into this step

2 - Data Preparation

+ Wrangle data and prepare it for training
+ Clean that which may require it (remove duplicates, correct errors, deal with missing values, normalization, data type conversions, etc.)
+ Randomize data, which erases the effects of the particular order in which we collected and/or otherwise prepared our data
+ Visualize data to help detect relevant relationships between variables or class imbalances (bias alert!), or perform other exploratory analysis
+ Split into training and evaluation sets

3 - Choose a Model

+ Different algorithms are for different tasks; choose the right one

4 - Train the Model

+ The goal of training is to answer a question or make a prediction correctly as often as possible
+ Linear regression example: algorithm would need to learn values for $$m (or W) and b (x is input, y is output)$$
+ Each iteration of process is a training step

5 - Evaluate the Model

+ Uses some metric or combination of metrics to *measure* objective performance of model
+ Test the model against previously unseen data
+ This unseen data is meant to be somewhat representative of model performance in the real world, but still helps tune the model (as opposed to test data, which does not)
+ Good train/eval split? 80/20, 70/30, or similar, depending on domain, data availability, dataset particulars, etc.

6 - Parameter Tuning

+ This step refers to hyperparameter tuning, which is an "artform" as opposed to a science
+ Tune model parameters for improved performance
+ Simple model hyperparameters may include: number of training steps, learning rate, initialization values and distribution, etc.

7 - Make Predictions

+ Using further (test set) data which have, until this point, been withheld from the model (and for which class labels are known), are used to test the model; a better approximation of how the model will perform in the real world

**Universal Workflow of Machine Learning**

In section 4.5 of [his book](https://www.amazon.com/Deep-Learning-Python-Francois-Chollet/dp/1617294438), Chollet outlines a universal workflow of machine learning, which he describes as a blueprint for solving ML tasks

> *The blueprint ties together the concepts we've learned about in this chapter:* ***problem definition, evaluation, feature engineering, and fighting overfitting***

How does this compare with Guo's above workflow? Let's have a look at the 7 steps of Chollet's treatment (keeping in mind that, while not explicitly stated as being specifically tailored for them, his blueprint is written for a book on neural networks)

1. Defining the problem and assembling a dataset
2. Choosing a measure of success
3. Deciding on an evaluation protocol
4. Preparing your data
5. Developing a model that does better than a baseline
6. Scaling up: developing a model that overfits
7. Regularizing your model and tuning your parameters

![](https://drive.google.com/uc?export=view&id=19em3BqCii5bY6mhtfAEN4gTCbbgy05Rg)

Chollet's workflow is higher level, and focuses more on getting your model from good to great, as opposed to Guo's, which seems more concerned with going from zero to good. While it does not necessarily jettison any other important steps in order to do so, the blueprint places more emphasis on hyperparameter tuning and regularization in its pursuit of greatness. A simplification here seems to be:


> *good model → *too good* model → scaled back, *generalizable* model*


**Drafting A Simplified Workflow**

We can reasonably conclude that Guo's workflow outlines a *beginner* approach to the ML process, more explicitly defining early steps, while Chollet's is a more advanced approach, emphasizing both the explicit decisions regarding model evaluation and the tweaking of models. Both approaches are equally valid, and do not prescribe anything fundamentally different from one another; you could superimpose Chollet's on top of Guo's and find that, while the 7 steps of the 2 models would not line up, they would end up covering the same tasks in sum

> *Mapping Chollet's to Guo's, here is where I see the steps lining up (Guo's are numbered, while Chollet's are listed underneath the corresponding Guo step with their Chollet workflow step number in parenthesis)*:

1. Data collection
→ Defining the problem and assembling a dataset (1)
2. Data preparation
→ Preparing your data (4)
3. Choose model
4. Train model
→ Developing a model that does better than a baseline (5)
5. Evaluate model
→ Choosing a measure of success (2)
→ Deciding on an evaluation protocol (3)
6. Parameter tuning
→ Scaling up: developing a model that overfits (6)
→ Regularizing your model and tuning your parameters (7)
7. Predict
~~~
It's not perfect, but I stand by it!
~~~
In my view, this presents something important: both workflows agree, and together place emphasis, on particular points. It should be clear that **model evaluation and parameter tuning** are important aspects of ML. Addition agreed-upon areas of importance are the **assembly/preparation of data and original model selection/training**

Let's use the above to put together a simplified workflow to ML, the 5 main areas of the ML process:


> 1 - **Data collection and preparation**: everything from choosing where to get the data, up to the point it is clean and ready for feature selection/engineering

> 2 - **Feature selection and feature engineering**: this includes all changes to the data from once it has been cleaned up to when it is ingested into the model

> 3 - **Choosing the algorithm and training our first model**: getting a *better than baseline* result upon which we can (hopefully) improve

> 4 - **Evaluating our model**: this includes the selection of the metric as well as the actual evaluation; seemingly a smaller step than others, but important to our end result

> 5 - **Model tweaking, regularization, and hyperparameter tuning**: this is where we iteratively go from a *good enough* model to our best effort

So, which approach should you use? Are there really any important differences? Do those presented by Guo and Chollet offer anything that was previously lacking? Does this simplified workflow provide any real benefit? As long as the bases are covered, and the tasks which explicitly exist in the overlap of the workflows are tended to, the outcome of following either of the 2 models would equal that of the other. Your vantage point or level of experience may exhibit a preference for one

**Conclusion**

As you may have guessed, this has really been less about deciding on or contrasting specific workflows than it has been an investigation of what a reasonable ML process should look like

![](https://drive.google.com/uc?export=view&id=1i7fzIUxz-oEs8V4uMdoZCQUl51NMrbVz)
