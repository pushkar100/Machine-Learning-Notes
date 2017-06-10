# DESCRIPTIVE STATISTICS NOTES (UDACITY CLASS)

# Lesson 1: Intro to Research Methods.

The 3 Factors that are always important to conduct a good research:
1. The size of the sample set (bigger the better)
2. The focus of the sample set (Ex: Asking *students* about exams)
3. The methodology used for surveying/conducting experiment (sound methodlogy)

## Constructs:

There are certain things for which there cannot exist just one method to correctly measure them. 
Examples of such things include happiness, guilt, memory, etc and they are known as **Constructs** (Very difficult to define and measure).

Using **Operational Definitions**, we can measure Constructs in the real-world. What is Operationa Definition?:
http://www.pqsystems.com/qualityadvisor/DataCollectionTools/operational_definition.php
(Operational definition removes ambiguity while measuring something that could be interpreted differently by different people.)

Operational definition:
- Is a way of turning constructs into variables we can measure, and
- A way of describing a variable in terms of the way we measure it.

Tip: 
- *Gallons of water* is NOT a construct since it can be easily measured in *gallons*. 
- *Age* is a construct since different people might consider age differently, like by DOB, Maturity, Height, etc.
- *Age by DOB* is NOT a construct since we can measure it by DOB.
- *Annual Salary* is a construct since different people might consider it differently, like by USDs, Yens, Property, etc.
- *Annual Salary in USD* is NOT a construct  since we can measure it in *USDs*.

## Variables:

A variable is a value that may change or differ between individuals in an experiment. Scores on an intelligence test qualify, since each person may have a different score.

**Note:** Statements about the relationships between variables are called **Hypotheses**. (Ex: 'Students who *sleep* more before an exam tend to get better *marks* in the exam').

## Extraneous Factors (Lurking Variables):

**Extraneous Factors** are those things that can influence Constructs. (Ex: Sleep factor before taking a memory test).
If a certain factor is made constant (Like conducting an experiment at the same time when time is considered as a factor), 
it is better for the outcome/conclusion. (Ex: If everyone takes a memory test at the same time [Acc. to their respective timezones] then the results can be trusted better.)

The more extraneous factors that are constant, the easier it is to trust the conclusion we arrive at from analysing the data. 
The reason for this is that these lurking variables usually ambush our results (if they keep varying between each item) (lurking to attack analogy).

## Population & Sample:

(Refer: https://classroom.udacity.com/courses/ud827/lessons/1293178557/concepts/565334210923)

Population is the entire set of items included in the experiment and the Sample is a subset of the population. 
The average result of the experiment for the population is known as `μ (myu)`. [Population average]
The average result of the experiment for the sample set is known as `x̅ (x bar)`. [Sample average]

**Note**: A population is a group of phenomena that have something in common. The term often refers to a group of people, as in the following examples:
- All registered voters in Crawford County
- All members of the International Machinists Union
- All Americans who played golf at least once in the past year

But populations can refer to things as well as people:
- All widgets produced last Tuesday by the Acme Widget Company
- All daily maximum temperatures in July for major U.S. cities
- All basal ganglia cells from a particular rhesus monkey

The average of the population `μ (myu)` could be the same as the average of the sample `x̅ (x bar)` but the opposite is seldom true since there 
would exist other samples within the population, some of which are mutually exclusive to the considered sample.
(So their average will not be the same).

Therefore, *generally* μ (myu) and x̅ (x bar) won't be exactly the same. Also, a *good* sample set is important to conclude a research.

A bigger sample will better approximate the population. Therefore, bigger samples are more useful.

### Sampling Error:

The difference between μ (myu) & x̅ (x bar) is called *Sampling Error* `μ - x̅`.

### Parameter v/s Statistic:

A parameter is a characteristic of a population, while a statistic is a characteristic of a sample.
Therefore, μ (myu) is a **parameter** and x̅ (x bar) is a **statistic**.

Also, the **number** of people/items included in the **sample** is denoted by `n` and going by the above definitions, `n` 
is also a **statistic**.

Refer: https://www.cliffsnotes.com/study-guides/statistics/sampling/populations-samples-parameters-and-statistics

## Visualizing Relationships:

When plotting a graph between data, we use the `x axis` to represent the *Independent Variable/Predictor Variable* and 
on the `y axis` we plot the *Dependent Variable/Outcome*.

An example of this is plotting 'Hours of sleep' on the x-axis (independent) and 'Memory Test Score' on the y-axis (dependent).

## Correlation Does Not Prove Causation!:

What this means is that even though there is a relationship between independent & outcome, it does NOT prove that 
the independent is the CAUSE for the outcome.

Example: If the relationship between sleep and memory score suggests that more sleep sees better memory scores, it does not mean that 
a person who has slept more will always score more (Someone who has slept less may still score the same). Therefore, the correlation 
CANNOT be cause for causation.

The reasons for this could be the existence of OTHER extraneous factors (Other lurking variables).

A fun example that shows correlation cannot prove causation is the **Golden Arches Theory**. 
(https://mediawiki.middlebury.edu/wiki/IPE/Golden_Arches_Theory_of_Conflict_Prevention) 
(Answer: Opening a McDonald's in other countries *cannot* be the cause for that country to not go to war with the USA).

**Note:** If there is a correlation, then we can *predict* something but *not prove it*.

### How to prove causation?

For showing a relationship/correlation, we need to undertake observational studies/surveys (like asking people as part of a survey).
In order to show causation, we need to perform a **Controlled Experiment**.

## Surveys v/s Controlled Experiments:

### Surveys: 

Advantages of surveys:
1. Surveys are inexpensive.
2. Easy way to get info on a population.
3. Can be done remotely. (via mail, for example.)
4. Anyone can access and analyze survey results. (They are timeless)

Disadvantages of surveys:
1. Biased responses.
2. Respondents not understanding the question. (1 & 2 can be called **Response bias** and is a negative aspect of a survey)
3. Untruthful responses.
4. Respondents refusing to answer. (It is known as **Non-response bias** and is a negative aspect of a survey)

Surveys are used to probe *Constructs* and these constructs can have a lot of definitions. Surveys need to contain carefully worded questions.

### Controlled experiments: 

The definition of a controlled experiment is a test where the person conducting the test only changes one variable at a time 
in order to isolate the results. An experiment where all subjects involved in the experiment are treated exactly the same 
except for one deviation is an example of a control experiment.

Basically, in controlled experiments, we control the variables/factors.

Example: Placebo: Give a random set of people a sleep pill (half the people get an 'active' pill and half get an 'inactive' pill). The 
experiment is to test whether the 'active' pill has an effect on the user's sleep. The participants are NOT told if they are receiving an active
pill or an inactive pill. The researchers want all the people to believe that they are taking medication(active pill). 
This process helps eliminate bias from the outcome. [The inactive pill is a **placebo** and the case where people who take the placebo and felt better 
is known as the **placebo effect**. If people know they are taking the placebo then they might subconsciously think that 
they are not doing anything and hence it will influence the results.]

Basically, placebos can help identify lurking variables(extraneous factors).

Note:
- Single Blind: Only the participants don't know which pill they are taking. 
- Double Blind: Even the researchers measuring the participants do not know which pills they have taken. 
(Double blind increases the accuracy of the experiment)

Extraneous factors need to be controlled in order to get causal results.

**Note:** In a controlled experiment, the researcher seeks to:
- Manipulate the independent variable.
- Measure the changes in the dependent variable or outcome.
- Control the extraneous/lurking variable.

## Random Assigment:

Random assignments could help **minimize** some of the lurking variables/extraneous factors. 

Example: Say an experiment needed to be done 
to measure if a pill had a certain effect on people. If a working pill was given to men alone and a non-working pill to women alone and 
the result showed men sleeping more, it could mean two things, either the pill worked or that women in general sleep more. This result would be 
inconclusive.

If the pills had been given out randomly, then both men and women would be a part of both the pill groups. This would lead to a better conclusion.

In a Random assignment, we: 
- Select individuals in such a way that everyone has the same chance of being selected.
- Select individuals in such a way that selection of one individual has no effect on anyone else's chances of being selected.

Random assignment works better on *larger samples* (closer to the population).

Examples where random assignment works well are Gender, Age, Wealth, etc (depending upon the context of the experiment to be conducted).

### Random v/s Convenience Samples:

Random samples are assumed to NOT be biased and treats every perso equally (like mentioned above). Convenience samples are the opposite of random samples since it forms the set of people who are conveniently picked (Example: Friends & relatives). They may be biased and not be representative of the population.







