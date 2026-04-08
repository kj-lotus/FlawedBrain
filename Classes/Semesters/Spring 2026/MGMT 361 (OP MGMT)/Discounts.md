![[Pasted image 20260403123752.png]]

### Quantity Discounts
- Discounts for ordering a full truckload of supply
- Discount for all units ordered over 100 unites
- Discount for the entire order if the order volume exceeds 50 units or $2000
- If EOQ >= discount threshold → Go ahead and order EOQ
- If EOQ < Discount threshold → Should we increase the order quantity to receive a discount yet incur a higher holding cost or should we order EOQ

EXAMPLE
	P = $2.5 per can  
	H = $2 per can per year  
	S = $1.6 per order
	Assume that you get a discount of 5% off the entire order if the order  
	exceeds 50 units. How many cans should you order?
		![[Pasted image 20260403124306.png]]
		Next calculate total annual cost with EOQ
		![[Pasted image 20260403124419.png]]
		Now we have to compare with minimum order quantity for discount - change q to 50
		Since its a 5% discount we take price per can and take away 5% of the cost
			2.5 x 0.95 = 2.375 
			Now we substitute q as 50 and p as 2.375 
			![[Pasted image 20260403124649.png]]
			As we can see the cost for ordering more cans is less, even though we are holding more cans it is still cheaper, so we want the smaller cost so we **DO TAKE THE DISCOUNT**

### Lead time and Reorder Point
- **Lead time** : Time between when an order is placed and when it is received
- **Reorder point**: Inventory level when an order should be places
![[Pasted image 20260403124935.png]]

- **When do you order?**: We order when the inventory is enough to cover the demand till product comes (Lead time)
- **Inventory ordering policy** : When to order and how much to order
- Policy [ROP, Q] when inventory is equal to ROP, order Q units
	- ROP = D x L
	- ![[Pasted image 20260403125620.png]]

**IN CLASS EXERCISE**
	![[Pasted image 20260403125435.png]]
	Inventory Policy 1
		[D x L, EOQ]
		[360 x 0,24]
		[0,24]
	Inventory Policy 2
		[360/360 x 2,24] : D is in unit per year so we need to convert to unit per day, 360 units 360 days means one unit a day, then we multiply by the LT which is 2 days giving us a ROP of 2
		[2,24]
	
