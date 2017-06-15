
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
The **margin of error** is defined as the absolute distance between the mean and the (2σ/√n) deviations (*Two standard deviations*).

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
