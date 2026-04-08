1/16
Continuous Random Variable 
	Can take on any value in an interval on the real line or in a collection of intervals
	typically we do not talk about the probability of a continuous random value at a PARTICULAR value
		P(x=x)=0 is uninformativ
	Instead, we talk about the probability of the random variable taking values within a given interval
		ℙ (𝑥! ≤ 𝑋 ≤ 𝑥^2) is meaningful to describe the distribution of 𝑋
	![[Pasted image 20260116093801.png]]
	Integrate the curve to find the area under the curve
		![[Pasted image 20260116093842.png]]

Normal Probability Distribution
	Most common distribution for describing a continuous random variable
		heights of people
		test scores
		rainfall amounts
		scientific measurements
	CENTRAL LIMIT THEORY - a large collection of independent random variables behaves similarly to the normal distribution which explains many real world phenomenon.
	![[Pasted image 20260116094129.png]]
		SD is outside of the square root in the denominator
			EXP = to the power of
	Normal distributions are symmetric with respect to the mean parameter = mew
		Skewness = 0
		Mean = median = mode = mew 
		Graph is bell shaped
		![[Pasted image 20260116094317.png]]
	The mean parameter mew can be greater than, less than or equal to 0

Excel Normal Dist
	![[Pasted image 20260116094617.png]]
		Make sure to use the False and True parts correctly

Calculating value in an interval
	P(x1<X<x2)
		P(X<= x2) - P(X<=x1)
		take the larger distance and subtract it from the shorter distance to find the distance between the two points thus giving us the interval
		EXCEL : NORM.DIST(x2, mean, stand_dev, TRUE) − NORM.DIST(x1, mean, stand_dev, TRUE)

Standard Normal Probability Distribution
	Z score
		![[Pasted image 20260116095240.png]]
		Calculates how many times of the standard deviation a select value deviates from the mean.
			Z score of higher than 3 or -3 is considered outlier
	Excel 
		![[Pasted image 20260116095358.png]]
		![[Pasted image 20260116095436.png]]

Inverse 
	find x from knowing probability
		Probabilistic question: 𝑋 ∼ 𝑁(𝜇, 𝜎) for 𝜇 = 36,500 and 𝜎 = 5,000. Find 𝑥 such that ℙ 𝑋 ≤ 𝑥 = 0.1
		NORM.INV(probability, mean, standard_dev)
		NORM.S.INV(probability)
		We mostly work with NORM.S.INV to find the 𝒛-value with a specific probability in the lower tail
		ℙ 𝑍 ≤ z_value = lower tail probability
	Knowing the X value we are able to find the Z score

t-distribution
	z score can only be calculated with population mean adn SD
	t-stat can be found with sample mean and sd but need degrees of freedon
		n-1
	Bell shaped
	Symmetric with respect to mean = median = mode = 0
	SD is strictly greater than 1
	![[Pasted image 20260116101934.png]]


