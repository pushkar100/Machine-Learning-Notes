# DESCRIPTIVE STATISTICS NOTES (UDACITY CLASS)

Prerequisite 1 for taking up the Machine Learning Course on Udacity.

# Lessons 1-3: Intro to Research Methods.

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

# Lessons 4-6: Data Visualization

## Frequency chart: 
A frequency table is a table that shows the total for each category or group of data. 
**OR**
A Frequency Table is a table that lists items and uses tally marks to record and show the number of times they occur.

### Frequency Count
A **frequency count** is a measure of the number of times that an event occurs.

### Relative Frequency:
The **relative frequency** of an event is defined as the number of times that the event occurs during experimental trials, divided by the total number of trials conducted.

To compute relative frequency, one obtains a frequency count for the total population and a frequency count for a subgroup of the population. The relative frequency for the subgroup is:

`Relative frequency = Subgroup count / Total count`

The above equation expresses relative frequency as a **proportion**. It is also often expressed as a **percentage**. Thus, a relative frequency of 0.50 (proportion) is equivalent to a percentage of 50%.

`percentage = proportion * 100`

**Note:**
- **All proportion are greater than or equal to `0` and less than or equal to `1` **
- **The sum of the proportions of all the items in the frequency table must be equal to `1`**
- **The sum of the percentages of all items in the frequency table must be equal to `100%`**

It is important how we group the data into a frequency chart - and it depends on how we want to view the data. (Example: If we want to see how many students watch Udacity videos from each country, we group the data country-wise on the frequency table. Similarly, if we want to view how many students view the videos from each continent, we'd group the data continent-wise.)

### Histograms:
We can build **histograms** (Similar to Bar graphs but divided by **ranges** on the `x-axis` and by the **frequency** on the `y-axis`) easily from a given frequency table/chart. 

Bar graphs have distinct values or categories on the x-axis (No ranges) and their order of appearance does not really matter whereas in a histogram the values are ranges (we can change the ranges to depict smaller or bigger groups of x-axis values) and their order of appearance does matter - *Only one order* (Ex:  11-20 interval should come before 21-30 interval).

- Histogram x-axis variable: Numerical & Quantitative (Ex: 0 to 100)
- Bar graph x-axis variable: Categorical or Qualitative (Ex: Asia, Europe, Africa, etc)

(Refer: https://www.mathsisfun.com/data/histograms.html)

The length of the ranges on the x-axis are known as **bin sizes** or **interval sizes**. The bin size should be optimal, not too small nor too big since it could become difficult to visualize the data. The bin/interval size must be the **same** for all the bins.

(Interactive Histogram: http://www.shodor.org/interactivate/activities/Histogram/)

Sometimes, in a histogram, we compromise detail for convenience. For example, trying to get the exact number of students whose age is less than 20 when the interval contains 20 (20 is within the bin and not at the boundary of the bin) inside it is not possible (although we can get a rough estimate).

- With frequency tables, we have exact counts, so we can always create the histogram. But not the opposite way around.
- With tables, you can add the frequencies in each bin. With a histogram, you don't always know the exact frequencies (Compromise detail for convenience).
- A histogram lets you visually see the shape of a distribution.

**Note**: When we make a bin size larger, more values will fall into that bin and hence, the frequency for that bin increases.

#### Uniform Distribution:

The uniform distribution gets its name from the fact that the probabilities for all outcomes are the same. Every outcome is equally likely to occur. 

The histogram for a uniform distribution will look like a *rectangle*. The frequencies of all the bins/intervals will be the *same (equal)*. For roughly uniform distributions, the frequencies will be very similar (in case they aren't the same).

A deck of cards has a uniform distribution because the likelihood of drawing a heart, a club, a diamond or a spade is equally likely. A coin also has a uniform distribution because the probability of getting either heads or tails in a coin toss is the same.

(Refer: http://study.com/academy/lesson/uniform-distribution-in-statistics-definition-examples.html)

#### Normal Distribution:
**Normal Distribution** is a function that represents the distribution of many random variables as a symmetrical bell-shaped graph.

Even on a histogram, the normal distribution would appear like a bell-shaped graph. It would be roughly symmetrical, tapering off at the extremes.

(Refer: http://whatis.techtarget.com/definition/normal-distribution)

#### Skewed Distribution:
Skewed distribution is the opposite of a normal distribution.

**Positively Skewed Distribution** on a graph means the frequencies are more on the **left side** than on the *right*. (Also known as **right-skewed** distribution)

**Negatively Skewed Distribution** on a graph means the frequencies are more on the **right side** than on the *left*. (Also known as **left-skewed** distribution)

**Note:** The "skew" does **not** refer to the peak but instead to the tapered side (known as the **tail**). Normal distribution has two tails, one on either side of the peak. In right/positive skew, the tail is more on the positive/right side of x-axis (greater values' side). In the left/negative skew, the tail is more on the negative/left side of the x-axis (lower values' side).

(Refer: http://www.statisticshowto.com/skewed-distribution/)

# Lesson 7: Working with Google Spreadsheets

Refer: https://classroom.udacity.com/courses/ud827/lessons/116708348/concepts/1164749820923

**Formulae: (To help you with statistics and google sheets):**
- **Mean** or sample mean is another term for sample average. Therefore, `mean = x̅ (x bar)`. (Sum of all the observed outcomes  from the sample divided by the total number of events)
- **Deviation** of a particular result is the difference between one particular value and the mean(x̅).
- **Squared deviation** of a particular result is the square of its deviation from the mean(x̅).
- **Variance** is the *Average* of the *Sum* of the *Squared deviations* divided by `n` (n = the count of the sample set). (In other words, variance is the average of the squared differences from the Mean.)
- **Standard deviation** is the *Square root* of the *variance*. The Standard Deviation is a measure of how spread out numbers are. Standard deviation is denoted by `σ (sigma)`.

**Bonus:**
- **Median** is the "middle" of a sorted list of numbers. To find the Median, place the numbers in value order and find the middle. 
- **Median in the case of even set of numbers:** With an even amount of numbers things are slightly different. In that case we find the middle pair of numbers, and then find the value that is half way between them. This is easily done by adding them together and dividing by two.

**Google sheets functions:**
- average()
- sum()
- sqrt()

# Lessons 8-10: Central Tendency

## Choosing a number to represent typical data:

There maybe more than one number used to represent typical data. Example: What is the typical salary of a post-graduate engineer? Often, we can use different types of numbers to answer such questions.

1. **Mode** is the value at which the *frequency is the highest*. **(OR)** The *most common value* is the called the mode. (The number that *occurs the most*)
	- On a histogram, this is the bin or interval for which the frequency is the *Highest*.  The mode occurs on the `x-axis`.
	- For a frequency table, it is the value with the highest frequency (count).
2. **Median** is the value in the middle of the distribution (already defined earlier - check).
3. **Average/Mean** is that specific spot which rests in the center of the distribution, which is the average of all the values (already defined earlier - check).

### Modes:
#### No modes:
Some distributions have no modes. Example: **Uniform Distribution**. Since all the bins' frequencies are the *same* there is not one value which occurs the most. Hence, no mode.

#### Multiple modes:
Some distributions have multiple modes.  These are called **Bi-modal Distributions**.

Example: Shoe sizes histogram - women mostly have size 7 and men mostly have size 9 (Therefore, we can see two humps on the graph, even though there is only one value with the highest frequency).

(Refer: http://www.statisticshowto.com/what-is-a-bimodal-distribution/)

**Note: Global Maxima v/s Local Maxima:**
- When we take the entire sample set and find one mode or peak (most commonly occurring value) then that value is known as the **Global maxima**.
- If we split the graph into regions (like in the case of shoe sizes for men & women example) and find the peak/mode for those regions separately then those values become the **Local maxima** for that respective region.

**More on modes:**
- The mode can describe any type of data - *Categorical(qualitative)* as well as *Quantitative(numerical)*.
- All scores in the dataset **DON'T** affect the mode. (For example: if mode value (say x)  has frequency 100 and another value (say y) exists with frequency 10. If we add another score to y, increasing it's frequency to 11, the mode value (frequency of x) does not change since it is still the highest. (Therefore, all scores do not affect the mode and it holds true for adding, deleting or modifying a score). - see outliers.
- There is **NO** equation for the mode.
- The mode is *likely to change* from one sample set to another. The mode *need not be same in all the samples*.
- The mode changes with the *bin/interval size* on a histogram: If the bin is made large enough, most values will fit in there and it will have the highest frequency, so the mode will be that bin. If made smaller, the mode might fit into some other bin instead of the current one. 

The **mode** is **not affected by outliers** at all! (see outliers under 'mean' section)

**Note:** Find mode on google spreadsheets: Use the `=mode(<range>)` function (Example: `=mode(A2:A28)` and hit <enter>.
(Or refer to this video: https://www.youtube.com/watch?v=TC0ZGYEf8dU)

### Mean:
Mean is the average of all the *sample* data.

`Mean = sum of all n sample data / n`. 

It has an equation and hence it is used alongside *mode* for data representation. **Mean/average** is represented by `x̅ (x bar)`

**Mathematical Equations for Mean:**

For a **Sample set**:
`x̅ = Σx / n`  
where `Σx` is the sum of all the values in the sample data set (`x1+x2+..+xn`) and `n` is the number of values in the sample data set. (Sample average)

For an entire **Population**,:
`x̅ = Σx / N`  
where `Σx` is the sum of all the values in the entire population (`x1+x2+..+xN`) and `N` is the number of all values in the entire population. (Population average)

**Notes on mean:**
- *All* the scores in the distribution *affect* the mean. (That is, the mean will change if we add an extreme value to the dataset. For example, adding 10000 to a dataset of 10 elements with a mean of 7 will change the mean drastically).
- The mean can be described by a **formula** (unlike mode).
- **MOST IMPORTANTLY: Many samples from the same population will have similar means** (unlike mode). (Explained in detail later - but this can be seen to be true with random samples).

#### Outliers:
**Outliers** are those values in data that can be *unexpectedly different* from the rest of the values.

For example, in the set 10, 96, 100, 5, 12, 67, 100000, 50 the value 100000 is the outliner because it is an extreme value w.r.t the other ones in the set. 

When outliers exist, the **mean will be greatly affected** and the mean will **not be an accurate representation of the data (misleading).** It makes the mean a lot less representative of the middle of the data.

A **median** might be more representative of the middle data. It is less affected by the outliers compared to the mean.

Note that the **mode** is **not affected by outliers** at all!

### Median:
The median is the middle value of a data set. But, it is not just any middle value - it is the middle value when the data set is **sorted into order**. From *least-to-greatest* or *greatest-to-least* - both orders are okay!

Example: Find median of 5, 3, 7, 10, 6?
Answer:  Sort them as 3, 5, 6, 7, 10. The middle value is 6. Median = `6`.

#### Median for even number of values:
When odd number of values exist, it is easy to pick the middle one after sorting them. But, for even set of values, there are two middle numbers (instead of just one). In this case, we find the middle point of those two middle numbers. That is, median will be the **average of the middle two values**.

Example: Find median of 5, 3, 7, 10, 4, 6?
Answer:  Sort them as 3, 4, 5, 6, 7, 10. The middle values are 5 & 6. Median = (5 + 6) / 2 = `5.5`.

**Note**:  Median is known to have a **Robust** tendency. What this means is that it is not affected much by departures from the norm (caused by outliers). Hence, it is more reliable than the mean to calculate the middle point of the distribution when data contains outliers. (Only slightly affected by outliers).

The median is generally used as a measure whenever we deal with *highly skewed distributions*.

**Formula for median:**
For an ordered(sorted) dataset `x1, x2, x3, .. , x(n-1), xn` the median is defined as:
- For odd elements: `Median = x(n+1/2)`, and
- For even elements: `Median = ( x(n/2) + x(n+1/2) ) / 2`.

**Finding the median on a histogram**:
Sum up all the frequencies. Find the median number (depending on odd or even ~= half the sum of frequencies). The value (of the bin) at the median number is the median.

### Mean, Median and Mode in Normal Distribution:
In a normal distribution, since the peak is in the middle the mode will be in the middle (highest frequency bin). Also, since the distribution is symmetric, the median and the mean will also be in the middle.

Therefore, `mean(x̅) = median = mode` for **Normal Distribution**.

### Mean, Median and Mode in Skewed Distribution:
In a Skewed distribution, the bin with the highest frequency will be to one side of the distribution. That bin represents the mode. 

The mean and median will be affected by the tail (outliers). But, the median being more robust, will not move towards the tail side as much as the mean does. 

Therefore:
- `mean(x̅) < median < mode` for **Negative Skewed Distribution**.
- `mode > median > mean(x̅)` for **Positive Skewed Distribution**.
(Sometimes they could be `<=` or `>=` also)
