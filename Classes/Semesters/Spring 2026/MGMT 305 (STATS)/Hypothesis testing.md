Testing for Means and Proportions

Hypothesis Testing
	used to determine whether a statement about a population parameter should or should not be rejected. 
	Null hypothesis H0
		tentative assumptions
	Alternative Hypothesis Ha
		Opposite of null hypothesis
	Hypothesis testing uses data from a sample to test the two competing statements H0 and ha
	Two outcomes
		Reject Null Hypothesis
		Fail to reject Null Hypothesis
	![[Pasted image 20260123094025.png]]

Null and Alternative about a population mean
	Equality part appears in the null hypothesis
	Hypothesis test about population mean takes 1 of the three forms
		![[Pasted image 20260123094137.png]]
		There is always an equals part to the equation, either less than or equal to, greater than or equal to, or simply just equal to.

Type 1 Error
	Rejecting H0 when it is actually true
	The probability of making a type 1 error when null hypothesis is true is called the significance (a) 
	Predetermined usually 1, 5 or 10% to control the probability of making a type 1 error

Type II error
	Accept null when it is false (reject Ha when Ha is true)
	Normally we do not control this probability
	Statisticians avoid the risk of making a Type II error by using “do not reject H0”  instead of “accept H0”.
![[Pasted image 20260123094631.png]]

Test Function
	Want to make a decision based on presented evidence
	Need mechanism that takes the sample values and significance level and provides a decision
	we would like this to be optimized and type II error minimal
Population mean when pop sd is unknown
	![[Pasted image 20260123095302.png]]
	H0: mean0=
	Need to use degrees of freedom to find t test stat
![[Pasted image 20260123095659.png]]
	All the alternatives to previously listed nulls
p-Value approach to one tailed hypothesis testing
	p value is probability computed using test statistic
		measures support provided by sample for null hyp
	![[Pasted image 20260123095924.png]]![[Pasted image 20260123100055.png]]
	The lower the p value the higher the probability taht Ha is true
	Excel =t.dist
	crit value is a point on horizontal axis = t.inv
	![[Pasted image 20260123101643.png]]
Tests about Population portion
	![[Pasted image 20260123102806.png]]
	![[Pasted image 20260123102826.png]]
	