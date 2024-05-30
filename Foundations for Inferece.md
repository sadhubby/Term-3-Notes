#csmodel 

Probability Distribution
- represents the probabilities of different possible outcomes for an experiment
- to preduct a variable accurately, understand the underlying behavior of the target variable
- knowing the probability distribution of the target variable is necessary
- determine the possible outcomes
- the probabilities should add up to 100. the close to 100, the more likely

The more trials we have, the closer we are to the 50% mark and the better we are at approximating 

## Normal Distribution

- ubiquitous distribution.
- arguably the most common
- unimodal, bell-shaped, symmetric

Has 2 Parameters:
- mean(mew) - the center of the distribution
- standard deviation (sigma) - the spread of the distribution
![[Pasted image 20240524144618.png]]
	changing the mean would change the most average, the peak of the curve. the peak of the curve is always centered at the most average.
- to describe a data point in the distribution, the data point is represented by how far does it deviate from the mean. to describe the data point is to describe how far it is from the mean. 
![[Pasted image 20240524144900.png]]

Distance cannot be simply used due to differences spread. Thus, normalizing the value based on the spread is needed. 
![[Pasted image 20240524145223.png]]
- In this case, we pick the one on the right because it is more dispersed, much farther from the mean. 

But the best way to describe a data point is using the z-score. The z-score is a standardized measure of how far a data point is from the mean

$z=\frac{(x-\mu)}{\sigma}$

We can also use percentile. The percentile of a data point corresponds to the fraction that lies below that data point. So if you say you are at the 67th percentile. Meaning that you are better than the 67%. 

Computing for percentiles is essentially computing the area under the curve which can be done with integrals. but in statistics, tables are usually used

Of course, real world data is not perfect normal distribution. Even though the data is not perfectly normal, we can still approximate it. This is called normal approximation. Normal distribution is a mathematical model that is often used to approximate the data. 

When to do normal approximation?
- use normal distribution to approximate the data if the data is nearly normal
- The Normal Q-Q plot is mostly straight
- Otherwise, using normal distribution may lead to non representative results
- ![[Pasted image 20240524150904.png]]

## Point Estimate

z-test; z-score
ch square; ch score







