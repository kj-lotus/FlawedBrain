	## Waiting time ##

Queueing System
	Input -> Buffer -> Processing
		Input: 
			Passengers in an airport, customers in bank, patients in hospital, callers at call center, 
		Buffer 
			Queue
		Processing
			Check in clerks at an airport
			Tellers at a bank
			Nurses at a hospital
			Customers service rep at call center
	Arrival rate (Demand Rate) = 1/ inter arrival time
		# flow units / time
		Process Capacity = Resource Capacity = 1/activity time (service time)
			Service Rate
				How fast you are serving a customer
		
CVa = StDev (inter-arrival times) / Average (inter-arrival times) - demand side
Cvp = StDev (process times) / Average (process times) - supply side
utilization = flow rate / process capacity
	(1/a) / (1/p) = p/a
	ASSUMPTIONS
		Arrival rate less than process capacity
			1/a < 1/p
![[Pasted image 20260223125745.png]]![[Pasted image 20260223130021.png]]

![[Pasted image 20260223131347.png]]
Class Example
	Utilization = p/a = 4.5/5 = 0.9
	Waiting time = 4.5 x (0.9/(1-0.9)) x ((1^2+1.39^2)/2) = 59.37 min 
	Total time = Tq + p = 59.37 + 4.5 = 63.87 min
	Customers In queue = Iq = r x Tq = 1/a x Tq = 12 * 59.37/60 = 11.87
	Customers in Service = Ip = u = 0.9
	Total Customers = I = r x T = 1/a x T = Ip+Iq = 12.77

In Class Exercise
	![[Pasted image 20260223131234.png]]
	![[Pasted image 20260223131251.png]]
		Utilization = p/a = 25/30 = 0.833
		CVa = 15/30 = 0.5
		CVp = 5/25 = 0.2
		Average time in office = 25 x (0.83/(1-0.83)) x ((0.5^2 + 0.2^2)/2) = 17.7
		# patiante waiting = rxTq = 1/a x Tq = 2 x 18.1/60 = 0.6
		# patients in service = Ip = r x p =2 x 25/60 = 0.83 = u
		# patients in total = I = Ip + Iq = 14.3
		