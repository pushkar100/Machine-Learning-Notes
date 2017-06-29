# Machine Learning - By Georgia Tech

A simple introductory course to Machine Learning offered by Georgia Institute of Technology on Udacity. 

Its prerequisites include: 
1. Intro to Descriptive Statistics
2. Intro to Inferential Statistics (or any elementary statistics course should do)
3. The course uses python, so we must be comfortable with python programming.

# Lesson 1: ML is the ROX

**Machine learning** is the broader notion of building computational artifacts learn over time based on experience.

Machine Learning involves **Computational Statistics.**

There are **3 parts** to Machine Learning:
1. Supervised Learning
2. Unsupervised Learning
3. Reinforcement Learning

**Supervised Learning:** Supervised learning is the machine learning task of inferring a function from labeled training data. The training data consist of a set of training examples. In supervised learning, each example is a pair consisting of an input object (typically a vector) and a desired output value (also called the supervisory signal).

Ex: labeled training data (input, output): `(1, 1)`, `(2, 4)`, `(3, 9)`, `(4, 16)`, etc.

So, for a new input `10`, we do this **Functional Approximation** by taking an input and guessing its output based on available training data. This is called Supervised Learning.

**Induction vs Deduction:** In supervised learning, we use the induction process to guess the new output, i.e we try to generalize output based on what we already know (Inductive Bias).

Induction example: The sun rose day before, yesterday and today. So, the sun will most likely rise tomorrow as well.

Deduction example: In deduction, we have rule(s) and whatever adheres to the rule is said to have been deduced. If `a => b` (a implies b) and if `a` is true then it implies `b` so `b` must also be true.

In Supervised Learning, we make use of **Induction**.

**Unsupervised Learning:** In unsupervised learning, there is no training data available. We have to come up with a structure to identify inputs based on the relaionships between the various inputs themselves. 

Example: We have a picture of a dog which has 4 legs. If given a picture of any other animal, the classifier classifies the new animal as a dog if it also has four legs as described for a dog. Just based on number of legs, horses, goats, etc are all classified as dogs. But, something like a car or tree won't be included in that group.

**Important!:** While Supervised Learning was about **functional approximation**, Unsupervised learnign is about **Description**.

We can combine the descriptive nature of unsupervised learning and the labeling mechanism of supervised learning: (Ex: Assume that we are trying to identify people from pictures and hence try to divide/classify them based on ethinicity, hair color, skin color, height, weight, etc. - we can divide them in any way and all these will be acceptable in some way or the other)

```
Pixels (input) ==> 
    Description [UNSUPERVISED LEARNING] ==> 
        Summaries (features of people) ==>
            Function approximation [SUPERVISED LEARNING] ==> 
                Labels (output)
```

**Reinforcement Learning:** In reinforcement learning, unlike the other two, there is no immediate feedback to let us know whether our choices are correct or not. The way it works is known as a **Delayed Reward System**.

For example: If we are playing a game of tic-tac-toe, supervised learning will have training data to help us with good or bad moves, unsupervised learning will also give immediate feedback but reinforcement learning will not tell us anything about the strength of the move we made until the end i.e until the game ends (win/lose). It is only after this outcome that for the next new game do we know whether that certain moves in the previous games led to a win or not (delayed learning/reward).

### Summary:
Every approach to ML is some type of **Optimization**.

- Supervised learning tries to label data well.
- Reinforcement learning tries to optimize behavior scores well.
- Unsupervised learning tries to make up some kind of criterion and develop clusters based on it. And, it tries to optimize the cluster scores well.

