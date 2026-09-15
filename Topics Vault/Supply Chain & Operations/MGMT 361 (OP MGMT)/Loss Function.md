---
topic: "Supply Chain & Operations"
related-topics: [Quantitative Methods & Statistics]
source-class: "MGMT 361 (OP MGMT)"
source-semester: "Spring 2026"
tags:
  - topic/ops
  - topic/quant
  - class/MGMT-361-OP-MGMT
---

Standard normal distribution
	Z ~ N(mean, stdev)
	![[Pasted image 20260327124139.png]]
	Step 1
		Find z score of critical ration from standard normal distribution function table
		![[Pasted image 20260327124413.png|380]]
	Step 2
		Convert z score into corresponding order quantity Q*
		![[Pasted image 20260327124503.png|241]]

Loss function for standard normal
	this time we use z score as the parameters (row and column) then you track down and side to side to find the value of the loss function
	To find expected lost sales we multiply stdev by L(zratio)
		![[Pasted image 20260327125821.png|465]]


![[Pasted image 20260327130008.png]]

z ratio = -0.54
loss = 0.7257
Expected loss sales
	9.52 * 0.7257 = 6.91 = 7
Optimal
	mean + zratio * stdev
	100 + (-0.54 x 9.52) = 94.86 = 95
Expected number of meals in shortage
	100 - 7 = 93 = expected sold
	expected unsold = 95 - 93.0913 = 1.9087
Expected meals wasted
	

---

## Related Notes

- [[Continuous Probability Distributions]]
- [[Class 2 - QM 306]]

