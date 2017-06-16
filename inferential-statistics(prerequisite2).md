
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

## Lessons 4-6: Hypothesis Testing

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
