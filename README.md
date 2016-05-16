# Naive-Bayes Algorithm
Implementing Naive Bayes Algorithm using iPython Notebooks

## What Is It?
The Naive-Bayes algorithm is an intuitive approach to making predictions based on prior beliefs or probabilities. Quoting Jason Brownlee, "it is the supervised learning approach you would come up with if you wanted to model a predictive modeling problem probabilistically".

Let's dive into the mathematics. We start off with a belief or a *prior probability* of event `A`. This is denoted as `P(A)`. Everything seems to be going well until we're hit with some new evidence `X`, which implies something about our belief. As much as we'd like to, we can't simply ignore `X` and go home. Instead, given evidence `X`, we must calculate a new value for event `A` called the *posterior probability*. This is denoted as `P(A | X)`. Finally, for the sake of completion, `P(X | A)` is the probability of observing evidence `X` for event `A` and `P(X)` is the untouched probability of observing evidence `X`.

![screen shot 2016-05-13 at 6 27 55 am](https://cloud.githubusercontent.com/assets/8285179/15245432/6b124518-18d4-11e6-8183-82bfe6247959.png)

You're probably wondering what makes this algorithm *naive*. Well, it's due to the underlying assumption that the probability of event `A` given any evidence `Xn` is totally independent of each other. This simplifies a lot of things and explains its popularity in many fields.

The content of this notebook uses Python to classify whether a patient is diagnosed with diabetes given a set of attributes. The data set is called the "Pima Indians Diabetes Data Set" provided by the National Institute of Diabetes and Digestive and Kidney Diseases.
