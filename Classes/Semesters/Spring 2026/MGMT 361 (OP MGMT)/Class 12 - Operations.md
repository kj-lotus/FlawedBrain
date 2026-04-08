### Multi Server Queue ###

Multi server
	m = number of servers in stage
	m>=1
	m x 1/p = Parallel resource - add capacity of each source)
	Be careful with M
Assumption: Demand < Supply
	1/a < 1/p
Flow Rate = min (demand, cap)
	= 1/a
	Implies utilization should always be less than 1
	Utilization = Flow rate / Capacity
		(1/a) / (1/p) = p/a
	Utilization with multiple servers
		Utilization = (1/a) / (m x 1/p)
			= p / a * m
![[Pasted image 20260225124316.png]]Tq = p x (u/1-u)x((CVa^2 + CVp^2)/2) SINGLE SERVER
![[Pasted image 20260225124703.png]]
###### the - 1 is OUTSIDE of the square root on u ######
	Do the power first then plug into formula
		power = sqrt(2(m+1)) -1

CVa = StDev (inter-arrival times) / Average (inter-arrival times) - demand side
Cvp = StDev (process times) / Average (process times) - supply side

![[Pasted image 20260225125222.png]]

State all variables
	a = 30
	std a = 15
		CVa = 15/30 = 0.5
	p = 25
	std p = 5
		CVp = 5/25 = 0.2
	m = 2
	Arrival time = 1/30 = 2 patient / hr
	Service rate = m x 1/p = 2 x 1/25 = 4.8 patient / hr
	utilization = p / m x a = 25 / 2 x 30 = 0.417
	Power = sqrt(2(2+1))-1 = 1.45
	Tq = 25/2 x (0.417^1.45 / 1- 0.417 ) x ((.5^2 + 0.2^2)/2)
		= 0.874594
	Total Time = Tq + p = 0.87 + 25 = 25.87 min
![[Pasted image 20260225130332.png]]
number of patients waiting = Iq = 1/a x Tq = 1/2(hour) * 0.87/60 (hours) = 0.03
number of patients in service = Ip = 2 pat/hr x 25/60 hr = 0.83 = 2 x u
number of patients in total = I = Iq+Ip = 0.03 + 0.83 = 0.86

![[Pasted image 20260225130726.png]]
Variables
	m = 80 (phones)
	25 customers / day = 1/a = 25/24
		a = 24/25 = 0.96 hr/customer
		CVa = 1
	p = 72 hr (service time)
		CVp = 100/72 (std p / p) = 1.389
	Utilization = p/m x a = 72 / 80 x 0.96 = 0.9375
	Flow rate = 1/a = 1/0.96 = 1.042
	Waiting time = (72/80) * ((3.75^11.728)/(1-80)) * ((1 + 1.389^2)/2) 
		=0.90 hours
	Inventory in service = Ip = m x u = 75
	Inventory in queue = 25/24 x 9.89 = 10.3 customers
	Total Inventory = Ip + Iq = 85.3 customers
