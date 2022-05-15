# MaximumLikelihoodApproach
<p>According to the central limit theorem, the distribution of a sample
variable approximates a normal distribution. This gives grounding in the
assumption that any continuous target variable could be represented as some
coefficient multiplied by a variable plus noise. It implies that target variables are
normally distributed with zero mean and some variance. Therefore, we are
composing a density function of a random variable. The density is also known
as likelihood. Hence, the aim is to maximize the likelihood function varying
weights and variance. It is worth saying that we also assume that the variables
are conditionally independent given the weight. Due to calculating reasons, we
are maximizing not likelihood itself but natural logarithm of likelihood function.
Taking partial derivatives with respect to weight and variance, the optimal
values of those parameters could be found. Performing some analytical
operations on weight and noise, there is a general trend that weight is usually
unbiased (it is not too low or too big), however, noise is biased to be too low.</p>
<p>Using log likelihood estimation, we are making too many assumptions. If
one of the conditions does not hold, the predictions stop being valid. Moreover,
it may happen that features are dependent on each other but calculating
likelihood there is a restriction on features being dependent. On the positive
side, likelihood allows us to predict not exact values but the range of values. In
particular, prediction is generated value plus squared noise. All in all, a model
significantly on particular distribution of the data which may cause problems
with predictions.</p>
