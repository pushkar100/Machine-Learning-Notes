
# Lessons 1-3: Estimation

### Point Estimate:
A single value given as an estimate of a parameter of a population.

As an example of a point estimate, assume you wanted to estimate the mean time it takes 12-year-olds to run 100 yards. The mean running time of a random sample of 12-year-olds would be an estimate of the mean running time for all 12-year-olds. Thus, the sample mean, M, would be a **point estimate** of the population mean, μ.

- The sample standard deviation (s) is a point estimate of the population standard deviation (σ).
- The sample mean (x̅) is a point estimate of the population mean, μ
- The sample variance (s2 is a point estimate of the population variance (σ2).

The estimate occurs as a result of point estimation applied to a set of sample data. Points are single values, in comparison to interval estimates, which are a range of values. For example, a confidence interval is one example of an interval estimate.

**Point estimates do not account for sampling error!**

#### Independent & Dependent Variables:

The independent variable here is the variable that we're hypothesizing changes or affects another variable.

The dependent variable here is the variable that we're hypothesizing is changed or affected by another variable.

### Margin of Error:
The **margin of error** is defined as the absolute distance between the mean and *two standard deviations*.

Therefore, margin of error contains **95%** of the values. That is, greater than `μ - (2σ/√n)` but less than `μ + (2σ/√n)`.

The interval is also know as **The 95% confidence interval for the mean**.

Further explanation: We have a sampling distribution (Mean of sample means) and we want to know if the mean of one of the samples(x̅) falls within the margin of error/95%confidence interval for the mean of means(μ). For the sample mean to be within it, it must satisfy the following inequality:

`x̅ - (2σ/√n) < μ < x̅ + (2σ/√n)`

We can list margin of error in terms of `z-score`: Since `1z = one standard deviation = σ/√n = covers 68%`, then `2z = two standard deviations = σ/√n = covers 95%`. 

To be precise, it is not 2 but `1.96` z-score for two standard deviations. 
Therefore, the margin of error/95% confidence interval lies between `-1.96` and `+1.96` z-scores of the mean.

**For Means of sample means:** 
95% of the sample means lie within 1.96 standard errors of the population. (1 standard error is the standard deviation on the sampling distribution).

**Note:**
- `+/- 1.96` are the **CRITICAL VALUES** of Z for **95%** CI.
- `+/- 2.33` are the **CRITICAL VALUES** of Z for **98%** CI.

### Formula for calculating Y% Confidence Interval:
The `x-axis` points `(x̅ - z(σ/√n)` and `(x̅ + z(σ/√n)` define the Y% Confidence interval where `z` is the z-score for that `x` value.

Also:
- `Confidence interval upper bound = sample mean + margin of error`
- `Confidence interval lower bound = sample mean - margin of error`

### Understanding Confidence Interval:
Let us take an example where a teacher has the mean marks of her students to be 68% (μ) with σ = 10%. She tries out a new interactive method of teaching with a sample of 25 students who get a mean mark of 75%. By finding the 95% confidence interval ({sample mean - margin of error, sample mean + margin of error}), we get to know that majority (95%) of students of the complete class (not just sample 25 students) will have mean marks between 71% & 79%. This is a 3-10% increase in the mean marks.

If the teacher continues the new way of teaching, **the mean exam score is likely to be between those bounds.**

# Lessons 4-5: Hypothesis Testing

### Levels of (Un)likelihood:
There are 3 levels of unlikelihood, known as **α (alpha) symbols**:
- `0.05` probability (5%)
- `0.01` probability (1%)
- `0.001` probability (0.1%)

If the proportion of something falls within these ranges, then the probability/likelihood of that occurring is "unlikely".

On the graph distribution, the **tail** part of the graph on the **positive side** (>95%) represents the "unlikely probability of occurring".

#### Critical Regions:
The regions of the graph that fall in the unlikelihood segment are known as critical regions.

The **critical regions** are defined as follows:
- Region with probability `>0.001` (corresponding to z-score `>3.08`)
- Region with probability `>0.1` (corresponding to z-score `>2.32`)
- Region with probability `>0.5` (corresponding to z-score `>1.65`)

The z-scores corresponding to these critical regions are known as `z critical values`. (i.e `3.08, 2.32, and 1.65`)

**Example:** If the probability of an event taking place has a z-score of 1.8 then we can say that the event is *only significant in the p < 0.05 region (where p = probability of event occurring)* (but not p < 0.1 and definitely not p < 0.01).

### Two Tailed Tests:
Instead of calculating the probability of top 5%, 1% or 0.1% as defined by the critical regions, we are sure that the bottom tail also is equally unlikely to occur.

Therefore, we can **split**:
- the top 5% to `bottom 2.5% and top 2.5%`
- the top 1% to `bottom 0.5% and top 0.5%`
- the top 0.1% to `bottom 0.05% and top 0.05%`

Now we have two symmetrical *tail regions* representing each critical region.

If the probability/percentage probability falls in *either of these tail regions* then it means that the value is *significant at that p < ProbabilityForThatCriticalRegion*.

Therefore:
- z-values for the `split 1% (+/-0.5%)` critical regions would be `+/-2.57`
- z-values for the `split 0.1% (+/-0.05%)` critical regions would be `+/-3.32`
- z-values for the `split 5% (+/-2.5%)` critical regions would be `+/-1.96`

#### Meaning of the tailed tests & significance of critical regions:
(Refer: https://classroom.udacity.com/courses/ud201/lessons/1335148547/concepts/1359192540923)

In a one tailed test or a two tailed test, the critical regions signify those values which are unlikely to occur. Therefore, if we get a value in these regions then it is unlikely that we got those values by chance.

When the mean of our sample falls **outside** the critical regions then it is known as **Null Hypothesis** `(H0)` and we usually denote it as `μ = μI` where μI is the μ after intervention - although μ is not exactly same as μI, it means that it is in the non-critical regions of μ.
- `μ = μI` refers to no significant change from mean.

**Intervention(`μI`)** here refers to the change we made to test the difference. For example, teaching a lesson to students(`μ`)  but trying a new method of teaching with songs so that students can remember better (`μI`). So, we try to check if `μI` is *signifcantly different* than`μ`.

**Null Hypothesis guesses that there will be *no* significant difference from the mean. ** That is, the effect of something new (or some change) will not improve or be reduced in a significant way.

When the mean of our sample falls **outside** the critical regions then it is known as **Alternate Hypothesis** `(HA) or (H1)` and we usually denote it as `μ > μI` or `μ < μI` or `μ != μI` where μI is the μ after intervention - It means that the mean is in the critical region of the distribution.
- `μ > μI` refers to positive significant change from mean.
- `μ < μI` refers to negative significant change from mean.
- `μ != μI` to either positive or negative significant change from mean.

**Note:** For a One-tailed test, the CR might be either the *lower tail* or the *higher tail*.

We usually consider **α (alpha) level of 5%**:
- `α = 0.05` and `z = 1.65` for a One-tailed test.
- `α = 0.05` and `z = +/- 1.96` for a Two-tailed test.
(`+/-2.5%` alpha level for a *two-tailed test*) 

#### How to Prove Hypotheses?:
We **cannot prove** that the *Null Hypothesis is true*. We can only *fail to reject it*.

For example, say H0 says that most dogs have 4 legs while HA says most dogs(>50%) have less than 4 legs. If we take a sample of 10 dogs and all of them have 4 legs then it means that we cannot reject our hypothesis of H0 and hence the **Null Hypothesis** must be *valid*. 

If 6 out of 10 dogs are three legged then can we prove that our Null Hypothesis `H0` is wrong? **YES**. Since >50% of dogs are three legged, we can **reject** our null hypothesis and favor the alternative one.

**Note:** 
- We cannot prove the Alternate Hypothesis either. Again, we can only fail to reject  it.
- **Importance of two-tailed tests:** We not only want to know if our intervention is causing an improvement but also if it is doing any harm. If we are trying to check for a positive difference and we get a negative one (or vice-versa) then it *does not just mean that our intervention is not working but is in fact counter-productive.*
- The exception to this advantage of two-tailed tests is in the case of, say, *a new treatment*. In this case, we only want to know if new treatment is better than the old. If it is worse then it does not matter since we would continue with the old treatment (Single tailed test is sufficient).
- **Rejecting the null** means that *we have seen significant change from the old mean w.r.t the new mean of the intervention test*. That is, new data lies in the critical region. We can *formally* define rejecting of the null by `p < probability for the selected α (alpha) level`

### Hypotheses Testing is Prone to Misinterpretations:
- If `H0` is **true** and we **reject** the null - It is a wrong decision. It is known as `Type I error`.
- If `H0` is **false** and we **retain** the null - Again, it is a wrong decision. It is known as `Type II error`

Example: H0 = Beverage is fine to drink now, HA = Beverage is too hot to drink now. 

- If you think the beverage is too hot and you wait to drink it but it turns out to be cold by the time you do so - You rejected H0 but H0 was true - Therefore: `Type I error`.
- If you think the beverage is fine to drink but it turns out to be hot and burns your tongue - You retained H0 but H0 was false - Therefore: `Type II error`.

# Lessons 6-7: t-Distribution:

We usually calculate the position of a sample mean on the distribution relative to the population mean `μ` and standard deviation `σ`.

Many times, we **do not know** the population mean and standard deviation. We only have a sample set of data with us. In this case, we cannot calculate the z-score (`(sample mean - population mean) / SE`) because *SE depends on σ* (`SE = σ / √n`).

We can use a new distribution known as `t-Distribution` which does **not** depend on `σ`. This `t-Distribution` is, however, more prone to error!

**t-tests are used when we do not know the population parameters whereas z-tests are used when we know them**

The **t-Distribution** is more *spread out* and *thicker in the tails* than a regular sample distribution (picture a normal curve but more spread out with the peak smaller than in a regular sample distribution).

**Calculating the `t-score`:**
- Since we are dealing with a sample and not population,  we have the Standard deviation of the sample: `S = √(Σ(xi - x̅)² / (n - 1))` (We use n-1 if it is sample and not population - bezzel's correction)
- Now, we can calculate the **t-score** as: `t = Mean Difference / SE`
- `SE` (Standard error) will depend on `S` and *not* the population std. dev. `σ`. 
- `SE = S / √n` (? re-check)

### Degrees of Freedom:
In statistics, the number of degrees of freedom is the *number of values* in the final calculation of a statistic that are *free to vary*.

**Example 1:** You have to choose `n` numbers. What is the degree of freedom?

Answer 1: We do not have any restriction on picking a number. So, while picking a number, we are free to pick any choice (vary). Picking each number adds to the Degree of freedom. Therefore, `DoF = n`.

**Example 2:** You have to map 3 subjects (a, b, and c) to 3 hours of study with each subject requiring one hour. What is the DoF?

Answer 2: The first slot can be either a, b or c (say, we select a). We have the freedom of choice. The second slot depends on what was selected for the first and are still left with two options (b and c). We have a choice between two (and say we choose b). Only for the last slot are we forced to select one (c). Therefore, `DoF = 2`.

**Example 3:** Choose n numbers (+/-) such that sum = 10. What is the DoF?

Answer 3: Let n = 4, assuming negative numbers are also allowed, we can choose any number as first. Second also has a choice. Third as well. But, fourth is forced. Therefore DoF = 4 - 1 = 3. In general, `DoF = n - 1`. Ex: Let x1 = 3(our choice). Now, x2 + x3 + x4 = 7. Let x2 = 10 (our choice). x3 + x4 = -3. Let x3 = 5 (our choice). x4 = -8 (forced). Only last number selected was forced.

#### Degrees of Freedom and Standard Deviation of a Sample:
When selecting data points for a sample from a population, we can choose any `n` values to construct a sample size of `n`. But, what about the mean of the sample (`x̅`)?

`( x1 + x2 + ... + xn ) / n = x̅`

Suppose we want a sample data set with a **particular** sample mean `x̅`. Then what is the DoF in selecting the `n` data points? 

`x1 + x2 + ... + xn = x̅.n`

We have to make sure that the *sum of the `n` values matches `x̅.n`. This is similar to the problem of selecting the `n` values that add up to a given sum. Therefore, `DoF = n - 1` (Since only last `n` value is a forced selection).

The reason why we use `n - 1` for calculating the SD for a sample set is because only these values vary instead of all them varying. (But, for a population we have all the values available and so we don't have to do any correction).

`S = √(Σ(xi - x̅)² / (n - 1))` for a sample where `S` is Std. Dev. of the sample.

### How to read the t-table:
How to read the t-table (It is different from z-table and uses degrees of freedom):? Refer: https://classroom.udacity.com/courses/ud201/lessons/1333678604/concepts/1470192730923

With a z-table, we found out the z-score and compared it to z-critical values. Using a **t-table**, we find out the **t-statistic** and compare it to the **t-critical values**.

**Note:**
- We can have **one-tailed tests** or **two-tailed tests** with `t-table` just like we did with the z-table scores.
- We can specify the `α` alpha levels (0.05, 0.01 ... etc) when calculating t-scores.
- `α` (alpha) levels indicate the area under the critical regions. Area/Proportion/Percentage/Probability.
- **Important:** If we are using the **two-tailed test** then we have to *split the α alpha value given by 2* and calculate the +/- t-scores for the same.

`t-table` column headers : Probability/α aplha levels/Proportion/Percentage

`t-table` row headers : Degrees of Freedom (which is `DoF = n - 1` for sample size `n`)

`t-table` cells : `t-scores` or `t-statistic`.

**Note: Calculating the t-statistic/t-score**
- `t-score` for the population `mean = 0`
- We *reject the null* if the `t-score`  is too far from the mean in either direction.
- `t = (x̅ - μ0) / SE` where `μ0` is population mean, x̅ is sample mean and SE is the *standard error (of the sample means)*.
- Remember that `SE = S / √n` where S is the std. dev. of the sample.
- Also remember that `S = √(Σ(xi - x̅)² / (n - 1))` since S is a std. dev. of the sample (and not the population).
- `x̅`  comes from population with mean `μ` and std. dev `σ`.

**Note:** 
- The **larger** the value of x̅, the stronger the evidence that: `μ > μ0` since t-statistic increases.
- The **smaller** the value of x̅, the stronger the evidence that: `μ < μ0` since t-statistic decreases.
- The **further** the value of x̅ from the mean `μ0`, the stronger the evidence that: `μ != μ0` since t-statistic is nowhere close to `0`.

Here, we represent the actual population mean as`μ0`. We use `μ` to depict the possible mean of the population assuming that the sample with mean `x̅` is an accurate representation of the population (`x̅ = μ`).

`t = (x̅ - μ0) / SE` is also known as **One sample t-test**.

For a **t-test**:
- The **null hypothesis** is `μ = μ0`
- The **alternate hypotheses** are: `μ > μ0`, `μ < μ0` and `μ != μ0`.
(Same as for z-scores)

**Note: Just like we calculated y% confidence interval using z-scores, we can calculate CIs using t-statistics as well.**

`Margin of error = CI / 2 = tc * SE = tc * (S/√n)` (Here, `tc` is the t-critical value)

`Confidence Interval (CI) = Mean +/- marginOfError = Mean +/- tc*(S/√n)` (Here, `tc` is the t-critical value)

(For confidence interval around population mean: use `μ` as mean, and For confidence interval around sample mean: use `x̅`  as mean)

**Note: Just like z-scores, we can think of t-statistics as the NUMBER OF STANDARD ERRORS.**

#### P-value:
P value (for a particular t-statistic) is defined as the probability of getting that t-statistic.

P-value represents the probability of getting a value *above* the positive value of the t-statistic (if positive tail is considered) in a  **one-tailed test.** .

P-value represents the probability of getting a value *below* the negative value of the t-statistic (if negative tail is considered) in a  **one-tailed test.** .

P-value actually represents the probability of getting a value *above* the positive value of the t-statistic and a value *below* the negative value of the t-statistic (i.e on both sides) of a **two-tailed test.**

**We reject the null hypothesis when the p-value is less than the `α` alpha level**

(Watch: https://classroom.udacity.com/courses/ud201/lessons/1333678604/concepts/1479057640923)

**Note: Cohen's d:**
`Cohen's d = (x̅ - μ0) / S` (Does not use standard error but std.dev. of the sample). It is a standardized mean difference that measures the distance between means in standardized units.

### t-tests for Paired Samples:
Until now we had been dealing with t-tests for **a** sample. Can we use t-tests to compare two samples? Yes! We can compare the differences between the two samples. Example: Difference between number of errors using a qwerty keyboard (sample 1) and using an alphabetical keyboard (sample 2). For paired samples, we take two samples and perform t-tests w.r.t the differences between the samples' values. We have a procedure for comparing the data from the two samples (particularly the **differences** between the values).

1. Within-Subject Designs:
	- Two conditions
	- Pre-test, Post-test
	- Growth over time (longitudinal study)

**Procedure:**
- First test values: `xi`
- Corresponding second test values: `yi`
- Difference between them: `Di = xi ~ yi` (Absolute difference)
- We find the mean (average) of the differences.
- Then we find the standard deviation (S) of the differences (from the mean of the difference). Procedure: Minus mean of diffs from each diff. Square them. Sum them up & divide by n-1 (since it is a sample). Taking square root of this should give us the standard deviation of the differences.
- We can calculate the the t-statistic as: `t = (x̅ - ȳ)/SE = (x̅ - ȳ)/(S/√n)` where `x̅` = mean of the 1st sample values and `ȳ` = mean of the 2nd sample values. `S` is the standard deviation of the differences between corresponding x and y values, found in the previous step. `n` is the sample size.
- Confidence Interval: `CI = (x̅ - ȳ) +/- Tc*(S/√n)` where `Tc` is the t-critical value for that confidence interval (Note: t-critical values are the limits of the CIs and it is not the t-statistical value that we calculate!).
- `x̅ - ȳ` is also known as the **Mean Difference**.

The **Null Hypothesis** can be written as `μ1 - μ2 = 0` (Both samples are similar) and **Alternate hypothesis** as `μ1 - μ2 != 0` (One sample is significantly different from the other). 

Another way of representing difference in hypotheses: `μD = μ1 - μ2`.
Therefore, **Null Hypothesis: `μD = 0`** and **Alternate hypothesis: `μD != 0`**.

**Note:** The paired sample tests involve **Dependent Samples**. Ex: Testing for errors on two types of keyboard.

# Lessons 8-9: t-tests part 2:

### Effect Size:
Effect size emphasizes the **size of the difference** rather than confounding this with sample size. Effect size is a statistical concept that measures the strength of the relationship between two variables on a numeric scale. The effect size is the difference between the critical value and the value specified in the null hypothesis.

- For a **z-test/t-test** effect size is the **mean difference** `x̅ - μ`.

Means differences are great for variables when we have easy-to-understand meanings. But, for variables which are not easy to understand, the mean difference is not very useful.

- There are other ways to calculate the effect size: **Standardized Difference**.

One of the standardized difference measures is called **Cohen's d** (Already defined).

- There are **Correlation Measures** as well.

**r^2** is a correlation measure which is the proportion (%) of variation in one variable that is related to ("explained by") another variable.

### Statistical Significance:
**Statistical Significance** is a hard-to-grasp term. It does **NOT** mean the followinf:
- Important
- Large or Sizeable
- Meaningful

**Statistical Significance** only means two (**correct**) things:
- We reject the Null Hypothesis
- Results are not likely due to chance (Not accidental nor due to sampling error)

### How to Determine Meaningfulness of Results?
Since statistical significance does not talk about the meaningfulness of results, there are a few points by which we can determine that for a result:
- What was measured? Variables - practical, social or theoretical importance .. ?
- Effect size - even a small effect size can be helpful
- Can we rule out random chance? Can we determine that the result is not due to sampling error?
- Can we rule out alternative explanations? Can we rule out Lurking Variables?

### Cohen's d (revisited):
Cohen's d is a standardized difference. That is because, like other standardized scores (like z-score), it calculates something, difference between means and puts the difference in terms of number of standard deviations.

`Cohen's d = (x̅ - μ) / S` where `S` is the standard deviation of the sample. 

### r^2:
r^2 is a correlation measure. It is also known as **Coefficient of determination**. r^2 values range from `0` to `1`. 

`r^2 = 0` means that the variables are not at all related.
`r^2 = 1` means that the variables are perfectly related. (Rarely happens in the real-world)

#### Computing r^2:
We can compute r^2 as follows:
- Calculate the *t-score* or *t-statistic* (`t`). Note that this is the t-score that we compute and is **not** the t-critical value (that is at the edge of the CI/alpha level)
- Determine the degrees of freedom (`df`) which is usually `n - 1` for sample size of `n`.
- Calculate r^2 from the following formula:

`r^2 = t^2 / (t^2 + df)`

(Ex: t = 1, df = 10, therefore r^2 = 1 / (1 + 10) = 1/11 = 0.091 = 9.1%)

#### Interpreting r^2:
If r^2 is `x%` then it means that x% of the variation in a variable can be explained by another variable.

### Writing Results of a Statistical Analysis:
Whenever we conduct a statistical study, we must list the results section as follows:

- Descriptive Statistics:
	- We have to mandatorily mention the mean and standard deviation
	- We can do this either by text,
	- or graphs (A histogram, for example),
	- or tables

- Inferential Statistics: Hypothesis testing (with alpha level mentioned)
	- What kind of test? Ex: One sampled t-test
	-  	statistic
	- df or degrees of freedom
	- p-value
	- direction of test (one tailed or two tailed?)

**OR:** 

- Inferential Statistics: APA (American Psychological Association) Style
	- `t(df) = x.xx, p = .xx, direction`
	- Example: `t(24) = -2.50, p < .05, one-tailed`

**AND Other things:** 

- Inferential Statistics: Confidence Intervals
	- Mention the confidence level. E.g: 95%
	- Lower limit (LL)
	- Upper limit (UL)
	- CI on what? Mention what the CI refers to.
	- One type of representation: APA Style: `x%CI = (LL, UL)` (Ex: `95%CI = (4, 6)`)
	- Altenative representation: `x%CI = (LL - UL)` or `x%CI = (LL to UL)`

- Effect Size Measures:
	- Mention Cohen's d or r^2 or both.
	- `d = x.xx`
	- `r^2 = .xx`
	
# Lessons 10-11: t-tests part 3:

### Advantages & Disadvantages of Dependent Samples:
Advantages:
- Controls for individual differences
- Use fewer subjects
- Cost-effective
- Less time-consuming
- less-expensive

Disadvantages:
- Carry-over effects: Second measurement can be affected by first measurement
- Order may influence results

Dependent Samples deal with **Within-subject designs**.

### Independent Samples:
Independent Samples deal with **Between-subject designs**. There are two ways in which we can do test independent samples:

- Experimental
- Observational

When comparing two samples (visualize two distributions), the difference is what matters: Refer https://classroom.udacity.com/courses/ud201/lessons/1330208559/concepts/1548634750923

`N(μ1, σ2) - N(μ2, σ2) = N( μ1 - μ2, √(σ1^2 + σ2^2) )` 

Explanation: When we subtract one normal distribution (`N`) with mean `μ` and `σ` from another, it results in another **Normal Distribution** with mean being the *difference in means of the two distributions* and the new standard deviation being  `√(σ1^ 2 + σ2^2)`.

**Note:**
- If the two are samples then the new SD `(S) = √(S1^2 + S2^2)`.
- The new distribution is more **spread out** than the original two graphs because the standard deviation for this graph is bigger than S1 (or σ1) and also bigger than S2 (or σ2).

**Standard Error (SE):** `SE = √(S1^2 + S2^2) / √n = √((S1^2 + S2^2)/n)`

**Standard Error (SE) when sample sizes are different (n1, n2):** `SE = √((S1^2/n1) + (S2^2/n2))`

**Degrees of Freedom (df):** `df = df1 + df2 = (n1 - 1) + (n2 - 1) = n1 + n2 - 2`

**t-statistic:** `t = Difference between means / Std. Error = (x̅1 - x̅2) / SE`


#### Pooled Variance (Sp^2):
When we are dealing with two samples, we can find something known as Pooled variance:

`Pooled Variance = Sp^2 = (SS1 + SS2) / df = (SS1 + SS2) / (df1 + df2)` Where `SS1` and `SS2` are sum of squared differences [`sum of all (xi-x̅)^2` like how you normally calculate for variance ] for samples 1 and 2 resp. and `df1` and `df2` are degrees of freedom for samples 1 & 2 resp.

**Corrected standard error (SE) using pooled variance:** `SE = √((Sp^2/n1) + (Sp^2/n2))` (Use `Sp` instead of `S1` and `S2`)

**Tough Question:** https://classroom.udacity.com/courses/ud201/lessons/1381238572/concepts/2529164880923
**Answer in Forums (Correct):** https://discussions.udacity.com/t/lesson-11-prob-2-t-statistic/90020/2

# Lessons 12-13: One-way ANOVA

### Intuition:
Assume we have 3 samples and we can do independent sample testing by computing 3 t-test scores and checking for statistical significance between any of them. This is a tedious task. There is a simpler approach.

Samples: A, B and C. t-tests required - A&B, B&C and A&C. Too many t-tests as number of samples increases.

**Number of t-tests** with `n` samples `= nC2 = n! / (n-2)!2!`.

t-tests basically measures the mean difference by standard error. Basically, `difference/error`. We can find a way to calculate the mean difference between more than 2 samples (>=2).

### Grand Mean (`x̅g`):
Grand mean (`x̅g`) is the **total mean of all sample means**.

#### Calculating the Grand Mean:
If sample sizes are **equal**: `x̅g = mean of sample means = (x̅1 + x̅2 + .. + x̅n) / n = mean of all values from all samples = (x1 + x2 + .. + xN) / N` where `n` is the number of samples and `N` is the total number of values in all of the samples together.

If sample sizes are **unequal**: `x̅g = mean of all values from all samples = (x1 + x2 + .. + xN) / N` where `N` is the total number of values in all of the samples together.

**Note: Between-Group Variability**
- **Smaller** the distance between sample means, the **less likely** population means will differ significantly.
- **Larger** the distance between sample means, the **more likely** population means will differ significantly.

**Note: Within-Group Variability**
- The **greater** the variability (spread of the sample distribution) of each individual sample the **less likely** that population means will differ significantly.
- The **smaller** the variability (spread of the sample distribution) of each individual sample the **more likely** that population means will differ significantly.

Between vs Within Group variability example: Treatment effects! Treatment effects would only increase variability between groups, not within a treatment group.

Difference in the means - The distance or variability between the means is the **average squared deviation of each sample mean from the total mean**.

### ANOVA:
ANOVA stands for **ANalysis Of VAriance**. And it is a measure of `difference / error` just like t-tests but useful while dealing with multiple samples of the same population (>=2). 

When the *number of independent variables* = `1` then we say we have **One-way ANOVA**. (Scope of this Udacity course is limited to One-way ANOVA)

For ANOVA Tests:
- `μ1 = μ2 = μ3 .. etc` will be the **Null Hypothesis (H0)**
- `At least one pair of samples is significantly different` will be the **Alternate Hypothesis (HA)**

**Note:**
- The **larger** the *within-group variability* (spread of distribution) the greater the lean towards *null hypothesis (H0)*.
- The **larger** the *between-group variability* (means of samples are further apart) the greater the lean towards *alternate hypothesis (HA)*.

**Important!:** The alternate hypothesis means that one pair of samples vary significantly. (**But we do not know which one** - to figure that out we must do some more tests.)

#### Statistic that includes between & within group variability: `F-ratio`

### F-Ratio:
The `F-Ratio` is a statistical measure that compares multiple samples by considering both within-group & between-group variability.

The *greater* the F-ratio the more likely we are to *Reject the Null (Reject H0)*.

`F = Between-group variability / Within-group variability`

**Exercise: Visualize statistical outcome - ** https://classroom.udacity.com/courses/ud201/lessons/1306898579/concepts/1611758350923

**Proper Formula:**
`F = [(n*Σ(x̅k - x̅g)^2) / (k - 1)] / [(Σ(x̅i - x̅k)^2) / (N - k)]` 

- `N` = Total number of values in all the samples combined.
- `n` = The sample size (All samples having *same size*).
- `k` = Total number of samples.
- `x̅k` = It is the sample mean of the sample that is being considered.
- `x̅g` = The Grand Mean.
- `F` is a ratio and it is **never** negative.

**F-statistic graph:**
https://classroom.udacity.com/courses/ud201/lessons/1306898579/concepts/1611758530923 (Positively skewed but not symmetric - only exists in the 1st quadrant of the graph)

The peak is `1`. That is, no difference between the group variabilities of between & within groups.

- **Sum of Squares for between samples** = `SS(btw) = (n*Σ(x̅k - x̅g)^2)` and `df(btw) = (k - 1)`
- **Sum of Squares for within samples** = `SS(wtn) = (Σ(x̅i - x̅k)^2)` and `df(wtn) = (N - k)`

Therefore, `F = [SS(btw) / df(btw)] / [SS(wtn) / df(wtn)]`.

**Mean Squares:** `MS(btw) = SS(btw) / df(btw)` and `MS(wtn) = SS(wtn) / df(wtn)`

Therefore, `F = MS(btw) / MS(wtn)`

**Also note:** 
- `SS(total) = SS(btw) + SS(wtn) = Σ(x̅i - x̅g)^2)` for all the values from all the samples.
- **When sample sizes are different**: `SS(btw) = Σ(nk * (x̅k - x̅g)^2)` when `nk`= sample size of the kth sample.
- **SS{within}** is also called **SS{error}** because this is the variation that can't be explained by the independent variable.

**Note**:
- DF for between-group variability `df(btw) = k - 1`
- DF for within-group variability `df(wtn) = N - k`
- Hence, `df(Total) = df(btw) + df(wtn) = N - 1 = All sample values - 1`

**Note**:
- `F` is a positive ratio.
- `F` can have only absolute values.
- The `F-critical` region lies to the positive side (right side of 1st quadrant).
- We can only have `one-tailed` & `positive` F-tests.

**Table** to find out f-critical values: http://www.socr.ucla.edu/applets.dir/f_table.html. We need two DFs - one for between grop variability (k-1) & one for within-group variability (N-k).

(How to read f-table: https://classroom.udacity.com/courses/ud201/lessons/1306898579/concepts/1611758820923)

# Lessons 14-15: ANOVA Continued

### Multiple comparison tests:
If ANOVA results show statistically significant differences between sample, we still *do not* which two samples are different.

We need to conduct additional tests to find out which two samples were statistically different and that it was *not* sampling error that caused the difference.

One of the tests is called **Tukey's Honestly Significant Difference (HSD)**.

`HSD = q * √( MS(wtn)/n ) = q * (Sp / √n)` 

- `q` is called the Studentized range, 
- `Sp` is the pooled variance, 
- `n` is the sample size.

Therefore, from above it is clear that `Sp = √(MS(wtn))`

Purpose of `q`: Adjust whole HSD so that it is less likely we commit a `Type-I` error (i.e: reject H0 when it is actually true).

(Table for calculating `q`: https://www2.stat.duke.edu/courses/Spring98/sta110c/qtable.html)

**Note:** On the table, `df` is the degrees of freedom for within-group variability.

**If two or more of the samples have an absolute difference greater than HSD, then their difference is said to be statistically significant!**. That is, if `mean(x̅) of test A ~ mean(x̅) of test B > HSD` then A & B are said to be *statistically different*.


**Drawback of Tukey's HSD:**
- We can only calculate it when *sample sizes* are all the *same* (`= n`).

### Cohen's D for Multiple Comparisons:
`d = (x̅1 - x̅2) / √(MS(wtn))` for comparison between sample 1 & sample 2.

### η^2 (Eta Square) for Effect Size:
`η^2` is another measure of effect size like ANOVA.

`η^2` tells us the proportion of total variation that is due to between-group differences (**Explained Variation**).

`η^2 = SS(btw) / (SS(btw)+SS(wtn)) = SS(btw) / SS(total)`

Example: If `η^2` is say `x%` then `x%` of the reason for the difference is due to the difference between groups (between samples).

Range of η^2: `0 <= η^2 <= 1`

### Assumptions in ANOVA:
- *Normality assumption*: The data from each sample fall along a normal curve.
- *Homogeneity variance:* The data come from populations with similar amounts of variability.

# Lessons 16-17: Correlation
Up until now we were talking about "one variable". What if the data we are analyzing contains two variables? In that case, we will need a new design - how we collect data, how we visualize data - but the way in which we analyze could still be the same.

We generally deal with two variables that are related like, height & weight, time spent studying & grades, etc.

One of the variables is assigned `x` while the other is assigned `y` (Convention).

`x` parameter is usually known as **independent variable**, **predictor**, or **explanatory**.

`y` parameter is usually known as the **outcome**, **response**, or **dependent**.

How do we define the relationship between the `x` and `y` variables?
- A strong relationship has a **direction**.
- **Positive relationship:** As `x` increases `y` also increases. *(+ve slope, upwards)*
- **Negative relationship:** As `x` increases `y` decreases. *(-ve slope, downwards)*

**Correlation** is a way to measure how to things are related to each other. Correlation is a statistical measure that indicates the extent to which two or more variables fluctuate together. A positive correlation indicates the extent to which those variables increase or decrease in parallel; a negative correlation indicates the extent to which one variable increases as the other decreases.

If two variables have a **strong relationship** then it means that they have a **high correlation.**

Correlation between `x` and `y` are usually depicted on **Scatter plots.**

(Watch & solve: https://classroom.udacity.com/courses/ud201/lessons/1345848540/concepts/1715827330923)

### Correlation Coefficient (`r`):
Correlation Coefficient (`r`) also known as **Pearson's `r`** is defined as:

`r = COV(x, y) / (Sx * Sy)`

`COV(x, y)` = **Co-variance** of x & y (i.e How much x & y vary together).
`Sx`  = **Standard deviation** of `x` values.
`Sy`  = **Standard deviation** of `y` values.

**Note:**
- `r` is **not** a percentage.
- `r^2` is the **percentage variation in `y` explained by the variation in `x`**.
- `r^2` is also known as the **coefficient of determination**.

**Note: values of r**
- Perfectly positive correlation (upwards, +ve slope) : `r = 1` (Ex: Age in years vs age in months)
- Perfectly negative correlation (downwards, -ve slope) : `r = -1` (Ex: Sleep hours vs awake hours)
- No correlation (randomly scattered) : `r = 0`
- *All other* correlations: `-1 < r < 1`
- The closer the `r` values to `1` or `-1` the **stronger** the correlation.
- The closer the `r` values to `0` the **weaker** the correlation.
- As sample size **increases** the `r` gets **smaller**.

#### Calculating Pearson's r in the Google Spreadsheet:
`=PEASRON(start cell for var x : end cell for var x, start cell for var y : end cell for var y)`

#### Step-wise calculation of correlation:
Refer: https://www.mathsisfun.com/data/correlation.html

**Note:** Our population data might have correlation but not our sample. This is one of the reasons for sampling error.

Which is why the **true correlation for population** is defined by **ρ** (rho). (`r` is the correlation between samples).

#### Hypothesis testing for correlation: 
- **Null Hypothesis (`H0`)** states: `ρ = 0`
- **Alternate Hypothesis (`HA`)** states: `ρ > 0`, `ρ < 0`, or `ρ != 0`

We hypothesize between populations (not samples) - hence, we used ρ.

**Hypothesis testing** can be done using the **t-statistics**:
- `t = (r * √(N - 2)) / √(1 - r^2)` where `N = all sets of x & y values`
- Degrees of Freedom: `df = N - 2` (Subtract one from each x & y values)
- We can use the `t-table` to get the `t-critical` values.
- We **can do** a non-directional (two-tailed t-test) (`ρ != 0`)

**Note:**
- If `t-statistic > t-critical` then we **reject the null**. 
- If `t-statistic > t-critical` then **there is a significant relationship between x & y**. 

### Confidence Interval for the True Correlation (CI for ρ):
- If CI includes `0` (Ex: {-.34, 0.41}) then we **cannot reject the null (retain it)**.
- If CI does **not** include `0` (Ex: {0.49, 0.566}) then we **reject the null**.

**Alternatively:** We can also find **p-values** and compare them against alpha levels (and either retain or reject the null).

### Re-iterating earlier proof: Correlation does imply causation!
(Refer: https://classroom.udacity.com/courses/ud201/lessons/1345848540/concepts/1715827820923)

It holds true when dealing with two variables also. For example, the reason why causation cannot be proved is because of **lurking variables (external factors)**, which could be anything, things that we don't even know.  For causation, the independent variable must occur before the dependent variable. Maybe there exists a LV `a` that affects both `x` & `y` that causes the correlation or `x` affects `a` which in-turn affects `y`. We may never know. (`a` is called the *mediator variable*). Hence, correlation cannot prove causation!

When we do not know which variable occurred first then there is something known as **Ambiguous Temporal Precedence**. To prove causality we need to know which one occurred first - and in this case, we can't prove causality. (Ex: A group of students take jazz class and really like. The teacher assumes his class caused them to like it. But, this need not be the case - since students who already liked jazz might have opted to take the class. Hence, the teacher's conclusion in support of causality is FALSE - **A Fallacy**.) 

Research terms such as **Post-hoc fallacy** & **Third variable problem**.

# Lessons 18-19: Regression
The straight line which we draw on the scatter plots to depict correlation is known as the **regression line** or **line of best fit** (It helps us define the relationship between x & y).

### Linear Regression:
The line of best first helps:
- Describe the data
- Make predictions (Marking a y value based on an x value with the help of regression line)

The **expected values** are represented by `ŷ` (y-hat) whereas the **observed values** are represented by `y`. Expected values are the ones that can be predicted from the line of best fit.

`Residual = Difference between observed & expected values`

### Symbolize Regression Equation:
- `y-intercept` is the point on the`y-axis` where the regression line passes through it.
- The `slope(m)` of the line is a measure of the angle at which the line cuts the y-axis. 

`slope(m) = changes in y for every 1 unit change in x = (y0 - yb) / (x0 - x1)` where `b` is the `y-intercept` .

**Equation for the regression line:**
`ŷ = (slope)x + yIntercept = mx + b`

If the *regression line* is for the **population**:
- `ŷ = (β1)x + β0` where `β1` is the *population slope* and `β0` is the population y-intercept.

**Note:**
- Slope (m) can be negative (-ve).
- Y-intercept (b) can be negative (-ve).

### Guessing the best fit line (Mathematically):
We need to find the exact `m` (slope) and `b` (y-intercept) that would help us identify clearly the regression line.

**How?:**
- One way is to **reduce** the **sum of residuals**.
- The residuals could be negative & cancel out.
- Therefore: we can work at reducing **Sum of Squared Residuals**. (`= Σ(y - ŷ)^2`)

**Calculate slope(m):**
The `slope(m) = r * (Sy/Sx)` where `r` is the correlation coefficient, `Sy` and `Sx` are standard deviations of `y` & `x` respectively.

**Calculate y-intercept(b):**
We need to find at least one data point that the regression line goes through and, along with slope, we can calculate the y-intercept.

**Slope(m) = The change in y after we change x by 1 unit = The additional difference in y when compared to x.**

**The y-intercept determines the minimum of the y-parameter it costs us every time & in all cases (independent of x-value). The slope on the other hand calculates the additional cost per change in x-value.**

### Errors in prediction:
Our predictions need not always match with observed/actual values. In fact, weakly scattered graphs will have more errors compared to strongly scattered graphs w.r.t prediction of value based on line of best fit.

Finding errors in prediction: **Standard error of estimate**

`Standard error of estimate = Sum of squared residuals / (N - 2)`
`Standard error of estimate = Σ(y - ŷ)^2 / (N-2)`

`N` is the total number of data points in the sample.

### Hypothesis Testing for Slope:
**"Are x & y linearly related?"**

`H0`: `β1 = 0` (β1 is the population slope)

`HA`: `β1 > 0` or `β1 < 0` or `β1 != 0` (β1 is the population slope)

### t-test for Slope:
**Note:** Always take the Degrees of Freedom (df) as `N-2`.

Given the alpha level & df, we can find the `t-critical` value.

The slope can be either negative or positive - Therefore, **two-tailed tests are possible**.

If `t-statistic > t-critical` then there is enough evidence to 1. Reject the null & 2. Suggest a significant relationship between x & y.

### Factors affecting Linear Regression:
**Outliers** affect most data analysis measures. In correlation, the correlation coefficent `r` was affected. Here, in regression the regression line can change drastically due to an outlier. We must identify the outliers before we perform regression analysis.

### Multiple Regression (Bonus):
Instead of having one predictor variable(x), we have multiple predictors (and one outcome(y)).

We still have one equation :  `ŷ = Ax1 + Bx2 + Cx3 ..` where A, B, C are "regression coefficients".

`R = multiple correlation co-efficent`
`R^2 = proportion of variability of y explained by our set of predictors`
