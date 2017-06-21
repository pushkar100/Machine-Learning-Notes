
# Lessons 1-3: Estimation

### Point Estimate:
A single value given as an estimate of a parameter of a population.

As an example of a point estimate, assume you wanted to estimate the mean time it takes 12-year-olds to run 100 yards. The mean running time of a random sample of 12-year-olds would be an estimate of the mean running time for all 12-year-olds. Thus, the sample mean, M, would be a **point estimate** of the population mean, μ.

- The sample standard deviation (s) is a point estimate of the population standard deviation (σ).
- The sample mean (x̅) is a point estimate of the population mean, μ
- The sample variance (s2 is a point estimate of the population variance (σ2).

The estimate occurs as a result of point estimation applied to a set of sample data. Points are single values, in comparison to interval estimates, which are a range of values. For example, a confidence interval is one example of an interval estimate.

**Point estimates do not account for sampling error!**

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

## Lessons 4-5: Hypothesis Testing

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
