1/14/26

Descriptive Stats
	- Measure of cnetral location
	- Variabliity
	- Distribution shape
	- etc
![[Pasted image 20260114064100.png]]
![[Pasted image 20260114064119.png]]

VARIABILITY
Concentration around the mean, 
	the more the values pile around the mean the less variability (skinnier curve vs fatter)
		Ideally less variability is better
	![[Pasted image 20260114064917.png]]

Tool for Variablity : Sample Variance
	![[Pasted image 20260114065128.png]]

It is squared so that the variance is always positive

n-1 in denominator used for samples but if you are finding for a population then use n as denominator

you can then find the standard dev 
![[Pasted image 20260114065415.png]]

SKEWNESS

the symmetry or assymetry of distribution curve
HOW TO CALCULATE
![[Pasted image 20260114065849.png]]
==EXCEL    =skew(array)==

If data skew right = positive value
If data skew left = negative value
If data is not skewed (symmetric) = 0
![[Pasted image 20260114070116.png]]

![[Pasted image 20260114070129.png]]
since median is farther to the right than the mean the skewness is negative
median > mean = negative


![[Pasted image 20260114070147.png]]

Since mean is greater than median the skewness is positive

median < mean = positive value

![[Pasted image 20260114070331.png]]

When skewness is calculated and is greater than 1 it is considered highly skewed


Z SCORE

![[Pasted image 20260114070712.png]]

x bar is the mean 
denominator (s) is the standard deviation
xi is the chosen data value - we can also find this using xi = xbar + z x s
to find on excel use = ===standardize(x, mean, standard deviation)==

Remember we can find the standard deviation using variability if needed

standard deviations used to find how far a data point is from the mean - related to the distribution curve percentages

OUTLIERS are considered when the z value is greater than or less than 3

EMPIRICAL RULE

related to z score to find how unusual for a given data value in a data set

![[Pasted image 20260114071406.png]]

REMEMBER the percentages take into consideration the positive and negative values of the stated standard deviation, if you want only the positive values make sure to divide by 2

![[Pasted image 20260114071633.png]]

