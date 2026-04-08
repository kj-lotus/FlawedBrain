#### Control Charts ####
X bar chart
	Detect Shifts in process mean
	Data points are sample means 
	We need 
		All sample means
		Mean of sample means (grand mean)
	Calculating Trial Control Limits
		Center Line (CL) = Grand mean
		Upper Control Limit (UCL) = Grand mean + A2R
		Lower Control Limit (LCL) = Grand mean - A2R 
	How to Find A2 Coeffecient
		Use Corresponding Sample Size
			Find number corresponding to that sample size
			![[Pasted image 20260304125532.png]]
	Example
	![[Pasted image 20260304130022.png]]
	A2 = 0.577
	UCL = 37.36
	LCL = 26.98
	**If any sample mean is outside of the UCL or LCL they are outliers**
	In this Example we have 5 outliers

R Chart
	Detect Increase in process standard deviation
	Data points are sample ranges
	We need
		All sample ranges
		mean of all sample ranges 
	UCL = D4R
	CL = Mean Range (R)
	LCL = D3R
		D4 and D3 are coefficients you find through a table
	![[Pasted image 20260304130352.png]]
		Same Logic
			Use n (sample size) to find corresponding value for D3 and D4

In Class Exercise
	![[Pasted image 20260304130709.png]]
	D3 = 0
	D4 = 2.115
	UCL = 19.04
	LCL = 0
	Outliers : 2,3,16
		We are looking at the range values for outliers not the mean
			Mean is found through the other UCL and LCL calculation using A2 coefficient
	

