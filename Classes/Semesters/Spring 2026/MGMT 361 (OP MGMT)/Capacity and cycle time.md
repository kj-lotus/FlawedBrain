1/23
Chipotle process
	![[Pasted image 20260123123710.png]]
	Stage 1 Capacity = M1 + M2
		1/activity time
			M1 = 1/50 (sec) - we want hour
				multiply by 60 then 60 again
					1/50 * 60 * 60 = 72 units/ hour
		M2 = 1/50 (sec) - we want hour
				multiply by 60 then 60 again
					1/50 * 60 * 60 = 72 units/ hour
		Stage 1 total capacity is 72 + 72 = 144 units/ hour
	Stage 2 Capacity
		M3 = 40 sec
			1/activity = 1/40
				convert to hours 1/40 * 60 * 60 = 90 units/ hour
	Bottleneck
		The bottle neck would be the stage with the lowest units/ hour
			Stage 1 is the bottleneck
	Process Capacity
		This is limited by the bottleneck
			90 units / hour
	Process designed cycle time
		1/process capacity 
			 = 1/ 90 unit per hour
				 multiply by 60 then again by 60 to get the seconds
					 40 units per second

Two Demand Scenarios
	![[Pasted image 20260123124519.png]]
	Scenario 1
		Demand rate in burrito/hr
			Demand rate = 1/ inter arrival time
				inter arrival time is how frequen 1 customer comes
					50 sec between each customer
				1/50 unit/sec
					convert to hours
						multiply by 60 then again by 60
							72 units per hour
								Previously we calculated that our Process Capacity is 90 units per hour
									We are able to support this demand rate
		Flow rate
			Number of customers the process actually can serve
				= whichever is the smallest either process capacity or demand rate
					in this case the demand rate is smaller
			Flow rate = 72 units per hour
	Scenario 2
		Demand Rate
			1/ inter arrival
				1/40 unit / sec
					90 unit per hour
		Flow rate
			Both demand rate and process capacity are equal
				We can produce maximum 90 units / hour
					Flow Rate = 90 units / hour
Gantt Chart
	Used to visualize resources
	![[Pasted image 20260123125635.png]]
		CHART
		![[Pasted image 20260123125650.png]]Each Color is a new customer
			Look carefully at the overlap
				Each customer comes in every 40 seconds, but it takes 50 seconds for each customer at the first stage
					We can see this overlap in M1 and M2 by 10 seconds
						This is our bottleneck and our process capacity
				Since it takes 40 seconds to pay, there is no overlap in M3 because their activity time is 40 seconds
	==ACTUAL CYCLE TIME = 1/FLOW RATE==
		UTILIZATION
			M1 = 5/8
				this is because M1 takes up 5 boxes and theres 8 total boxes until they get a new customer
			M2 = 5/8
				Same thing, 5 boxes out of the 8 boxes from start till new customer
			M3 = 100%
				They are always working there are no gaps 4 boxes are filled and theres only 4 boxes till


