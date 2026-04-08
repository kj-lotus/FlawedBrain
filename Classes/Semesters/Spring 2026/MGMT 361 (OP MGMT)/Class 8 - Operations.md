## Batching and Setup Time##
Batch Operations
	Batch
		Collection of flow units that are processed during one production or service cycle
		Multiple units in one batch
			can be delivered at same time or delivered continuously
		Starting a new batch needs a new setup
			Usually required by the resource
		Setup takes time
	Example : Baking Cookies
		![[Pasted image 20260204124009.png]]
Baking Cookies - Single product type
		10 min to prepare, 15 minutes to bake a tray
			12 cookies per tray
				oven can only hold 1 tray at a time
		Capacity depends on batch size
			Batch size = 1 tray: 1 tray takes 10+15 = 25 min
				Capacity = 60/25 = 2.4 tray/hr
		Capacity increases when batch size increases
	Production Cycle
		setup + baking time
		10 + 15 = 25 min
		we call it a cycle because it repeats
		each tray takes 25 minutes due to the 10 minutes it takes to prep and 15 minutes it takes to bake
	Capacity = how many trays of cookies you can get divided by the time it takes to get the cookies
		capacity = batch size (1 tray) / production cycle time
			how many units you can get in a certain amount of time
				1 tray / 25 minutes
					multiply by 60 to gets tray per hour
						60/25 = 2.4 tray / hr
	Now we change batch size to 2 trays
		2 trays consecutively
	Production Cycle:
		Setup - 10 min
		1st tray bake - 15 min
		2nd tray bake - 15 min
	2nd cycle
		Setup - 10 min
		1st tray bake - 15 min
		2nd tray bake - 15 min
	Set up time stays the same
		Baking time doubles because we are making 2 trays
	Production cycle time = Setup + 1st tray + 2nd tray
		10+15+15 = 40 min
	Capacity = batch size (2 trays) / production cycle time (40 min)
		1/20 tray / min
			1/20 * 60 = 3 trays / hr
	Can continue to add more and more trays
		3 trays
		10 min setup
		15 min bake for each tray
		Production cycle time = 10+15+15+15 = 55 min
		Capacity = 3/55 * 60 = 3.27 tray/hr
	Batch size increase causes capacity to increase too

Batch size and Capacity
	production cycle time = setup time + batch cycle * time per unit
	![[Pasted image 20260204125628.png]]

Producing Car Doors = Multiple Product Types
	Flow unit: a pair of doors (one left, one right)
	Setup machine for left doors - 50 min
	Produce left doors - 2 min
	Setup machine for right door - 50 min
	Produce right door - 2 min
	Production Cycle Time = 104 min
		![[Pasted image 20260204131023.png]]
	In class Exercise
	TEMPLATE
	# of pairs
		Total time per batch
			Capacity
	25 pairs
		100 + 4* 25 = 200 min
			25 / 200 * 60 = 7.5 pairs / hr
	50 pairs
		100 + 4 * 50 = 300 min
			50 / 300* 60 = 10 pairs / hr
	150 pairs
		100  + 4 * 150 = 700 min
			150 / 700 * 60 = 12.86 pair / hr	
