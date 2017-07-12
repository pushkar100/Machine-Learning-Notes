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

# Lesson 2: Supervised Learning 1 - Decision Trees

There are typically two types of supervised learning:
1. Classification
2. Regression

**Classification** is the process of taking an input and mapping it to a *discrete set of labels*, like true or false.

Example: Mapping a picture of a person (input) to a discrete set of labels - i.e Male or Female. Other types of discrete labels include car or airplane, true or false, etc (anything we might imagine).

**Regression** is more about *continuous valued functions*. (Unlike the discrete nature of classification). Given a bunch of points, we want to map a new value to a point. We will have a line depicting the existing values and the new value will be a point on that line. (That line represents a continuous function).

Classification vs Regression:
- Classification is mapping input to one of a samll set of outputs. (Output = discrete values)
- Regression is mapping input to a real number (potentially to one of an infinite set of real numbers). (Hence, Output = continuous values).

Examples:
```
Input: Credit score (Related to bank account)
Output: Lend money/not?

Type: Classification
```

```
Input: Picture of a person
Output: High school/college student/graduate?

Type: Classification
```

```
Input: Picture of a person
Output: Age? (age can be fractional too)

Type: Regression (Could be a any age - continuous range)
```

```
Input: Picture of a person
Output: Age in years (and nobody lives above 150)

Type: Classification 
(Age values are discrete - not continous - 
and the upper limit is 150 so the output 
is a very large discrete set of years of size 150)
```

## Classification Learning:
Some important terms related to classification:
- **Instance**: It is basically the **input** (or whatever makes up the input). Ex: Pixels of a picture, credit score indicator like money in the bank, etc.
- **Concept**: It is a **function** that **maps** an object (**input**) to the one item from a set of **outputs** (discrete set of values in case of classification). Ex: You are given an object and you need to tell us whether it is a car or not. (Usually, we deal with binary outputs in classification - like true or false - although we can work with more values as well). Intuitively, a concept is an idea and the function here represents that idea (Ex: maleness or femaleness of a person based on his picture - the function tells us that / maps it).
- **Target Concept**: The only difference between a concept and a target concept is that target concept is the thing we are trying to find i.e it is the actual answer. Ex: A function that tells us whether the object is a car or not? Out of all the concepts (functions) that might map the input to one of a set of outputs, the target concept is the answer (or mapping) that **we** are looking for! (Target concept is a specific idea)
- **Hypothesis (or Hypothesis Class)**: It is the set of all concepts that you are willing to entertain (Subset of concepts). We can use the *set of all concepts* as the hypothesis class - but this might make it hard for us to pick the concept we are interested in, the target concept, with limited or finite amount of data. One more way to think of it is that if we include all the mappings/concepts/functons we get a continuous set of outputs - and this represents regression not classification. 
- **Sample**: Sample is the **training set** (for supervised learning). What is a training set? It is the **set of all inputs that paired with a label**. Ex: Picture of a man paired with a label that says he is a man. Other examples: {Brown Hair color, woman}, etc.
- **Candidate**: It is the concept that *we think* might be the target concept. (Ex: assuming that if there is curly hair then the person is credit worthy - can get loan from bank).
- **Testing Set**: Testing set helps us determine if our candidate concept is right or wrong. Testing set looks exactly like the training set. We go through all the data in testing set, apply it to the candidate concept and compare it to the actual values of the testing set - to see if candiate predictions were right or wrong.

**All these terms will be clear once we start understanding specific problems over the next few lessons**

### Decision Trees
Let us take an example: You are on a date and come up to a restaurant. You need to decide if you want to enter that particular restaurant. The input to decide are the *features* of that restaurant. Output is if we must *enter or not*?.

The above example is a *classification* problem - binary outputs {enter, do not}. Hence, it is a binary classification problem.

Features of the restaurant (input):
- Type: french, thai, indian, etc.
- Atmosphere: fancy, hole-in-the-wall, casual.
- Restaurant is occupied or not?
- Hot date you want to impress or not?
- Cost: How expensive is it?
- How hungry are you?
- Is it raining outside or not? .. etc.

First, we need to ++represent++ our Decision Tree and only then can we think about the ++algorithm++ to work with the tree.

#### Representation of Decision Tree:

![](https://databricks.com/wp-content/uploads/2014/09/decision-tree-example.png)

A decision tree is like a normal tree data structure. 

Decision Tree consists of the following:
- It has nodes (points) and edges.
- The **nodes** refer to the **attribute** or behavior. (Ex: A node can refer to hunger - "Hungry or not?")
- The **edges** represent the **values** for an attribute. (Ex: One of the edges from the 'hunger' node will have a value 'true' and the other will have a value 'false')
- Root node is the top-most node of the tree. We traverse the tree from the root (i.e **Top-down** & not bottom-up)

The Decision Tree allows us to ++ask a series of questions (starting from the root) and based on the answers(values) we eventually end up choosing a path leading to a specific output++.

**Example of a testing set:** We feed data from our testing set to the decision tree to get the output:

Ex:

![](http://cdn.guru99.com/images/1-2015/012715_0719_DecisionTab3.png)

(In the above image, fly from & fly to are inputs while outcome is whether we have a flight for the inputs or not - the inputs can be fed to a decision tree to get the output)

**Note:** Whenever we construct a decision tree, we may or may not include all the input features in the selection. Therefore, whatever tree we get is a specific decision tree - hence, it becomes a **Candidate concept**.

(Refer: https://classroom.udacity.com/courses/ud262/lessons/313488098/concepts/3140257630923)

#### Writing an Algorithm to work with Decision Tree:
Every question that we ask needs to further narrow down the possibilities of the outcome. For example, if we are playing a game of 20 questions then a good first question would be 'animal or not?' - this reduces your concerned space to living things or inanimate & plant objects. A good second question could be 'person or not?' - again narrowing down the possibilies. The last guess could be the name of the person (Ex: 'Michael Jackson') but the same question is not a good first question since it fails to narrow down the possbilites especially if your guess is incorrect.

**An approach to picking a good Decision Algorithm:**
1. Pick best attribute (Ex: Best is one that splits data into roughly two sets).
2. Ask a specific question.
3. Follow the answer path.
4. Repeat first step (for another attribute) until we get an answer.
5. The only thing to keep in mind is that for constructing a decision tree, we need to go down the paths of all attribute values to get all possible outcomes (whereas when traversing an already built tree we would be going down only onw specifi path based on specific values).


