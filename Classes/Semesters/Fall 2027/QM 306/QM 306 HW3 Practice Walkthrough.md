---
tags: [qm306, linear-programming, solver, sensitivity-analysis, practice]
course: QM 306
topic: Make or buy LP with sensitivity analysis
---

# QM 306 HW3 Practice Walkthrough (Make or Buy LP)

This is a **parallel practice problem** built to mirror the structure of HW3 part by part, with different numbers. Work through this one, then do the Riverbend problem yourself in Excel using the same moves. Answers here will NOT match the homework.

Related: [[04b Linear Programming Applications]] · [[03 Solving LPs with Excel Solver]]

---

## The practice problem

Northgate Print Shop must fill every order it receives each month. Three products make up all of its work. A job done in house uses press time and finishing time, both limited. Any job not done in house is sent to an outside printer that charges a flat price per job and uses none of the shop's own time.

| | Flyers (A) | Brochures (B) | Posters (C) |
|---|---|---|---|
| Jobs required per month | 2,500 | 1,800 | 1,200 |
| Press minutes per job | 10 | 8 | 18 |
| Finishing minutes per job | 5 | 7 | 9 |
| In house cost | $18 | $30 | $50 |
| Outside printer cost | $35 | $55 | $78 |

Available each month: **60,000 press minutes** and **30,000 finishing minutes**. Goal: fill all jobs at minimum total cost.

---

## Part (a) Formulation

### Big idea

This is a **make or buy** problem. For each product you need two decision variables: how many you make in house and how many you send out. That is exactly like the Silver Star Bikes example in 04b needing two variables per item per period.

### Decision variables

- $I_A, I_B, I_C$ = number of Flyer, Brochure, Poster jobs done in house
- $O_A, O_B, O_C$ = number of Flyer, Brochure, Poster jobs sent to the outside printer

### Objective function (minimize total cost in $)

$$\min Z = 18I_A + 30I_B + 50I_C + 35O_A + 55O_B + 78O_C$$

### Constraints

1. Press time: $10I_A + 8I_B + 18I_C \le 60{,}000$
2. Finishing time: $5I_A + 7I_B + 9I_C \le 30{,}000$
3. Flyer demand: $I_A + O_A = 2{,}500$
4. Brochure demand: $I_B + O_B = 1{,}800$
5. Poster demand: $I_C + O_C = 1{,}200$
6. Nonnegativity: all variables $\ge 0$

> [!tip] Why the outsourced jobs are not in the resource constraints
> The outside printer uses none of the shop's time, so the $O$ variables only show up in the objective and the demand constraints. Same deal with the reference lab in HW3.

### Excel layout tips (color code)

Use one consistent color key and put a small legend on the sheet.

| Component | What goes there | Suggested color |
|---|---|---|
| Parameters | the data table (times, costs, demand, capacities) | light blue |
| Decision variables | 6 changing cells (in house row and outside row) | yellow |
| Constraints | LHS formulas with SUMPRODUCT next to the RHS | light green |
| Objective | one SUMPRODUCT cell for total cost | orange |

Solver settings: Min the objective cell, changing the 6 variable cells, add the ≤ and = constraints, check **Make Unconstrained Variables Non Negative**, method **Simplex LP**. Then select **Sensitivity** in the reports box when Solver finishes.

---

## Part (b) Sensitivity Report (what Solver gives you)

### Variable cells

| Cell | Final Value | Reduced Cost | Objective Coef | Allowable Increase | Allowable Decrease |
|---|---|---|---|---|---|
| In house A | 2,500 | 0 | 18 | 1.444 | 1E+30 |
| In house B | 1,800 | 0 | 30 | 3.222 | 1E+30 |
| In house C | 544.44 | 0 | 50 | 28 | 2.6 |
| Outside A | 0 | 1.444 | 35 | 1E+30 | 1.444 |
| Outside B | 0 | 3.222 | 55 | 1E+30 | 3.222 |
| Outside C | 655.56 | 0 | 78 | 2.6 | 28 |

### Constraints

| Constraint | Final Value | Shadow Price | RHS | Allowable Increase | Allowable Decrease |
|---|---|---|---|---|---|
| Press minutes | 49,200 | 0 | 60,000 | 1E+30 | 10,800 |
| Finishing minutes | 30,000 | -3.111 | 30,000 | 5,400 | 4,900 |
| Demand A | 2,500 | 33.556 | 2,500 | 980 | 1,180 |
| Demand B | 1,800 | 51.778 | 1,800 | 700 | 842.86 |
| Demand C | 1,200 | 78 | 1,200 | 1E+30 | 655.56 |

> [!note] Reading the signs in a MIN problem
> A shadow price of **-3.111** on finishing means one more finishing minute changes total cost by -$3.11, so it **saves** $3.11. 1E+30 just means "infinite."

---

## Part (c) Optimal solution and value

- In house: 2,500 Flyers, 1,800 Brochures, 544.44 Posters
- Outside: 0 Flyers, 0 Brochures, 655.56 Posters
- **Minimum total cost = $177,355.56**

> [!question] Why Posters get split
> Savings per job from doing it in house: A saves $17, B saves $25, C saves $28. But what matters is savings per minute of the scarce resource (finishing). A saves 17 ÷ 5 = 3.40 per finishing minute, B saves 25 ÷ 7 = 3.57, C saves 28 ÷ 9 = 3.11. C is the worst use of finishing time, so it is the one that gets partially sent out. Try this same check on HW3, it tells you which panel should be the "split" one.

---

## Part (d) Binding constraints and slack

- **Binding:** Finishing (uses all 30,000). All three demand constraints are equalities so they are always binding.
- **Non binding:** Press time. Used 49,200 of 60,000, so **slack = 10,800 minutes**. Shadow price is 0 because extra press time would sit unused.

---

## Part (e) Cutting the non binding resource (range of feasibility)

Press has an allowable decrease of 10,800, so press time can drop to 60,000 minus 10,800 = **49,200** with nothing changing.

**Case 1: press drops to 52,000.** That is inside the range (52,000 is above 49,200). You are just eating into slack. Same solution, same cost of **$177,355.56**.

**Case 2: press drops to 45,000.** That is below 49,200, outside the range. The sensitivity report cannot tell you the answer, so you **re-solve in Solver**. New result:

- In house A 2,500, B 1,800, C 311.11 and outside C 888.89
- Cost = **$183,888.89** (up $6,533.33)
- Now press becomes binding and finishing picks up slack.

> [!tip] The move
> Inside the allowable range: use the shadow price. Outside it: change the RHS and re-run Solver. Say which one you are doing and why.

---

## Part (f) Changing the binding resource

Finishing shadow price = -3.111, allowable decrease 4,900, allowable increase 5,400.

**1,500 fewer finishing minutes.** 1,500 is within the 4,900 allowable decrease, so the shadow price holds.
- Cost change = 1,500 × 3.111 = **+$4,666.67**, new cost **$182,022.22**
- Solution changes (binding constraint moved): in house C drops to 377.78, outside C rises to 822.22.

> [!warning] Common mistake
> Within the range, the **shadow price stays the same** but the **variable values still change** when a binding constraint moves. Only the non binding slack case leaves the solution untouched.

**8,000 extra finishing minutes.** 8,000 is more than the 5,400 allowable increase, so the shadow price only holds for the first 5,400 minutes. Re-solve:
- In house A 2,500, B 1,800, C 1,144.44 and outside C 55.56
- Cost = **$160,555.56**
- Press is now binding and finishing has 2,600 minutes of slack. If you had just multiplied 8,000 × 3.111 you would have gotten $152,466.67, which is wrong. The last 2,600 minutes are worth $0.

---

## Part (g) Should you buy extra capacity?

Suppose a vendor offers up to 8,000 extra finishing minutes.

**At $3.50 per minute:** Each extra minute only saves $3.11 (shadow price), and that is the best case. Paying $3.50 to save $3.11 loses money. **Don't buy.** (And past 5,400 minutes each minute saves $0.)

**At $2.50 per minute, buy 5,000 minutes?** 5,000 is within the 5,400 allowable increase, so the shadow price applies to every minute.
- Savings = 5,000 × 3.111 = $15,555.56
- Cost = 5,000 × 2.50 = $12,500
- **Net gain = $3,055.56, so yes buy.**

> [!tip] Decision rule
> Buy if price per unit < |shadow price|, and only for the amount inside the allowable increase.

---

## Part (h) Reduced cost questions

**At what outside price would the shop send out any Flyers?** Outside A has a reduced cost of 1.444, meaning its cost must drop by more than $1.44 before it enters the solution. So the outside printer would need to charge less than 35 minus 1.444 = **$33.56** per Flyer job.

**How much would in house Brochure cost need to change before sending Brochures out?** In house B has allowable increase 3.222. If its in house cost rises by more than **$3.22** (above $33.22), sending some Brochures out becomes cheaper. Direction: **increase**.

> [!note] Same answer two ways
> Outside B's reduced cost is also 3.222. Makes sense: making in house more expensive by $3.22 or outside cheaper by $3.22 closes the same gap.

---

## Part (i) Range of optimality on a cost coefficient

Outside C (currently used, 655.56 jobs) has objective coefficient 78, allowable increase 2.6. So the plan stays optimal as long as the outside Poster price stays at or below 78 + 2.6 = **$80.60**.

**Price rises to $80.** Inside the range. Same plan, but cost goes up because you still buy 655.56 outside:
- New cost = 177,355.56 + 655.56 × 2 = **$178,666.67**

**Price rises to $82.** Outside the range, so re-solve:
- New plan: in house A 1,320, B 1,800, C 1,200 and outside A 1,180
- Cost = **$179,060**
- Posters become expensive enough to bring fully in house, and Flyers get pushed out instead.

> [!tip] Inside vs outside the range
> Inside: same variable values, cost changes by (price change × amount of that variable). Outside: re-solve and describe the new plan.

---

## Checklist for doing HW3 yourself

- [ ] Six variables (in house and reference lab for each panel)
- [ ] Demand constraints are **=**, resource constraints are **≤**
- [ ] Color legend on the sheet, formulation in a textbox
- [ ] Sensitivity report generated and on the same sheet or right next to it
- [ ] For every what if: check the allowable range FIRST, then either use the shadow price or reduced cost, or re-solve
- [ ] Each problem on its own worksheet
