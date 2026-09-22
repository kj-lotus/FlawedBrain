---

## tags: [econ301, managerial-economics, lecture-notes, fundamentals] course: ECON 301 - Managerial Economics instructor: Professor Ben Zou term: Fall 2026 topic: "Topic 1: The Fundamentals of Managerial Economics"

# Topic 1: The Fundamentals of Managerial Economics

This lecture sets up the whole course. Everything later (demand, production costs, market structure, pricing, game theory) gets built on top of these seven ideas. If you actually understand these seven principles at a gut level, the rest of the semester is mostly "apply these tools to a new situation."

## The 7 Principles of Effective Managerial Decision Making

1. Identify goals and constraints
2. Recognize the nature and importance of profits
3. Understand incentives
4. Understand markets
5. Recognize the time value of money
6. Use marginal analysis
7. Make data driven decisions

Below, each one is broken down in depth, with the worked examples from lecture explained step by step rather than just stated.

---

## 1. Identify Goals and Constraints

Every decision maker, whether it is a person or a firm, needs a clearly defined goal before "good decision making" even means anything. You cannot optimize toward a fuzzy target.

For a firm, the assumed goal in this course is:=

> The firm's overall goal is to maximize profit.

That is the baseline assumption you will use in nearly every model this semester unless a problem tells you otherwise.

But goals alone do not determine outcomes. Firms (and people) face **constraints** that make the goal harder to reach. Two big constraint categories mentioned in lecture:

- **Available technology** — the production methods and know how you actually have access to. You cannot produce output methods that do not exist yet or that you cannot access.
- **Prices of inputs** — labor, materials, capital all have a price, and that price limits how much you can produce for a given budget.

The mental model here: goal maximization always happens _subject to_ constraints. This "maximize this, subject to that" framing shows up over and over in economics (utility maximization subject to a budget, cost minimization subject to an output requirement, and so on). Get comfortable with that structure now.

---

## 2. Recognize the Nature and Importance of Profits

This is the densest section of the lecture, so it gets the most space here.

### The basic profit equation

Profit maximization means:

```
Max Π = TR − TC
```

Where Π is profit, TR is total revenue, and TC is total cost.

**Worked example (Lamar's lemonade stand):** Lamar sold 50 cups of lemonade at $3 each, and spent $40 on cups, lemons, sugar, and water.

```
Π = TR − TC
Π = (50 × $3) − $40
Π = $150 − $40
Π = $110
```

That $110 looks like the full story, but it is not, because it only counted the cash he spent (an **explicit cost**). Keep this example in mind, it gets revisited below once we bring in opportunity cost.

### Accounting profit versus economic profit

This distinction is one of the most important ideas in the whole course, and it is genuinely a little counterintuitive the first time you see it, so slow down here.

**Accounting profit** = total revenue − total explicit costs This is the number your accountant or tax return would show. Explicit costs are actual cash outlays: rent, wages, materials, and so on.

**Economic profit** = total revenue − total explicit costs − total implicit costs Economists add one more category: **implicit costs**, meaning the value of opportunities you gave up by choosing this activity instead of the next best alternative.

Because implicit costs are almost always positive (there is almost always something else you could have been doing), **economic profit is usually smaller than accounting profit**.

The lecture's illustration of this idea: if a friend says "I'll pay for your lunch, it's free," is it really free? In an accounting sense, yes, you paid $0. In an economic sense, no, because you spent an hour of your time sitting there that you could have spent doing something else valuable. The "free" lunch had an implicit cost even though no cash changed hands.

### Opportunity cost, in depth

This is the concept that ties the whole section together, so here is the full definition:

> **Opportunity cost** = the value of your best alternative = explicit (monetary) cost + implicit (foregone opportunity) cost

A few things that make this concept click:

1. **It is always about the single best alternative, not every alternative.** If you turn down three job offers to take a fourth, your opportunity cost is only the value of the best of those three, not all three added together.
2. **Costs you'd incur no matter what you choose do not count.** The lecture poses this exact question: if you spend $30 a day on food whether you study abroad or stay home and intern, does that $30 belong in your opportunity cost calculation? No. Since it is spent identically under both options, it does not change based on your decision, so it is not part of the _differential_ cost of choosing one option over the other. Opportunity cost is about what changes because of the choice, not everything you spend regardless of the choice.
3. **Sunk costs are explicitly excluded from opportunity cost.** More on this below, because it deserves its own explanation.

**Worked example (opportunity cost of college):** Suppose four years of college costs $10,000 a year in tuition and $1,250 a year in books, and going to college means giving up a job paying $40,000 a year.

```
Tuition: $10,000 × 4 = $40,000
Books:   $1,250 × 4  = $5,000
Forgone salary: $40,000 × 4 = $160,000
Total opportunity cost = $40,000 + $5,000 + $160,000 = $205,000
```

Notice this number is much bigger than "sticker price" tuition. This is exactly why economists insist on opportunity cost thinking: the true cost of a decision is almost always larger than the cash you hand over, because it also includes what you gave up.

### Sunk costs and the sunk cost fallacy

A **sunk cost** is a cost that has already been incurred and cannot be recovered no matter what you decide going forward. The key insight, and the one that trips people up constantly in real life:

> Rational decision making should completely ignore sunk costs. Only the marginal benefit versus marginal cost of your choice _right now_ should matter.

Why? Because the money or time is already gone regardless of what you choose next. Bringing it into your current decision does not get it back, it just distorts your thinking about the decision in front of you.

But people do not actually behave this way, which is why it is called the **sunk cost fallacy**: treating money or effort already spent as a reason to continue an activity, even when continuing is a bad idea going forward.

The concert ticket scenario from lecture is a great gut check for this: you bought a $50 ticket weeks ago, but on the day of the show you are sick and it is raining. The $50 is spent no matter what you decide tonight. So the only question that should matter is: given how you feel right now, is going to the concert worth it? A rational decision maker asks that question and ignores the $50 completely. (And the lecture notes that your answer might change if the ticket had been free, which is itself revealing, since it means the $50 sunk cost actually was influencing the decision even though rationally it should not.)

Other sunk cost fallacy examples from lecture:

- An entrepreneur who has already lost $50,000 in a failing restaurant puts in another $20,000 because "I can't waste everything I've put into this." The $50,000 is gone either way, the only real question is whether the _next_ $20,000 is a good investment on its own merits.
- Sitting through a bad movie because you already paid for the ticket. Amos Tversky's line, as told by Michael Lewis, captures the rational response perfectly: "They've already taken my money. Should I give them my time, too?"
- An NFL team keeping an underperforming player because of the high draft pick spent on them. The pick is spent no matter what, the only real question is whether this specific player, going forward, is better than the alternatives.

There is even an old saying that captures the fallacy itself: "In for a penny, in for a pound," meaning people feel that since they are already partly committed, they should fully commit. Economically, that reasoning is a trap.

**Revisiting Lamar's lemonade stand with opportunity cost:** Lamar's time was not free just because he did not pay himself a wage. Suppose his best alternative use of that time was playing Madden, which he values at $30 worth of enjoyment. That $30 is an implicit cost of running the lemonade stand, so:

```
Π (economic) = ($3 × 50) − $40 − $30 = $80
```

Notice this is lower than the $110 accounting profit calculated earlier. That $30 gap is exactly the implicit cost of his time, which accounting profit ignores completely but economic profit captures.

### The Five Forces Framework: what determines whether profit can be sustained

Even if a firm is profitable today, will it stay profitable? This framework (adapted from Michael Porter's Five Forces) gives five factors that determine whether profits are sustainable in the long run.

1. **Entry** — how easy is it for new competitors to enter the industry? The lower the barriers to entry, the harder it is to sustain profit long term, because new competitors will rush in and compete away your excess profits. Food trucks are easy to start (low barrier, profits get competed away fast). Building a new high powered computer chip company is very hard to start (high barrier, easier to sustain profit).
    
2. **Power of Input Suppliers** — how much leverage do the people who sell you your inputs have? If input markets are concentrated (few suppliers), those suppliers can charge you more, squeezing your profit. Example: if there were only one lemon producer in the world, they could charge you whatever they wanted for lemons. Similarly, if labor unions gain more bargaining power, workers can negotiate higher wages, which raises your costs.
    
3. **Power of Buyers** — how much leverage do your customers have? If buyers are concentrated or have low switching costs (easy to go elsewhere), they can push your prices down, which reduces your ability to sustain profit.
    
4. **Industry Rivalry** — how intensely do existing competitors fight each other? More intense rivalry (price wars, low price guarantees, low product differentiation) erodes sustainable profit. Think Coke versus Pepsi, or Trader Joe's versus a discount grocer, constantly undercutting each other on price or marketing.
    
5. **Substitutes and Complements**
    
    - **Substitutes**: goods that can replace one another in use (butter and margarine, Netflix and Hulu, two apple varieties). The more substitutes exist, the less pricing power you have, since customers can simply switch away, which limits sustainable profit.
    - **Complements**: goods that are consumed together (fries and dipping sauce, shoes and socks, movie tickets and popcorn). Complements actually help you, since strong complementary products make your product more valuable. A lack of complements hurts you: if you make a game console but few developers make games for it, that console is much less attractive, which limits your ability to sustain profit. Netflix benefited early on from being the only major streaming complement to broadband internet, but the more competing streaming services appeared, the harder it became to sustain outsized profit.

The unifying theme of all five forces: anything that gives _other people in your market_ more leverage over you (easier entry, powerful suppliers, powerful buyers, tough rivals, easy substitutes) erodes your ability to hold onto profit over time.

---

## 3. Understand Incentives

The core idea, stated simply: **people respond to incentives**, and they respond in a fairly predictable way: they take an action whenever its marginal benefit to them exceeds its marginal cost to them.

Examples from lecture:

- **Sales commissions** incentivize workers to put in more effort (a personal cost to them), because it is now paired with a personal financial benefit that scales with effort.
- **Ticket inspection frequency**: increasing how often inspectors check tickets on a train raises the expected cost of riding without a ticket, which incentivizes more people to actually buy tickets.

Inside a firm, incentive design is a core job of a manager: structuring pay, bonuses, and monitoring so that employees' personal incentives line up with the firm's goals.

### Perverse incentives

A **perverse incentive** is an unplanned, usually negative, side effect of an incentive scheme. The incentive technically "works," in the sense that people respond to it rationally, but it produces the opposite of the intended outcome because the designer did not think through all the ways people could respond.

Two vivid historical examples:

- **The Window Tax (England, 1696):** landlords were taxed based on how many windows their property had, the idea being that more windows signaled more prosperity, so it was meant as a rough wealth tax. Since landlords were the ones paying, they responded rationally: many simply bricked up windows or built new houses with fewer windows to begin with. The tax did not capture prosperity the way intended, it just changed architecture.
    
- **The Great Hanoi Rat Massacre (1902, French colonial Vietnam):** the government paid a bounty for each rat killed, and people had to present a severed rat tail as proof. The incentive was "kill rats." What people actually did, since only the tail was checked, was cut off tails and release the (still alive) rats back into the wild, so the rats could keep breeding and produce more tails to cash in later. The incentive rewarded _producing tails_, not _reducing the rat population_, and people optimized for exactly what was measured rather than the underlying goal.
    

The lesson generalizes far beyond rats and windows: whenever you design an incentive, people optimize for the letter of the incentive, not necessarily the spirit of what you actually wanted. This idea shows up again later in economics and business as "you get what you measure."

### How people actually respond to incentives: three research examples

These are worth understanding conceptually since they show incentives are not always simple or intuitive.

**1. Fines as prices (Gneezy and Rustichini, 2000, day care study).** Some day cares had a problem with parents picking their kids up late. The day care introduced a $5 fine for late pickups, expecting late pickups to decrease. What actually happened is that late pickups _increased_. The explanation: before the fine, parents felt a moral or social obligation to be on time. Once a fine was introduced, picking up late stopped feeling like violating a social norm and instead felt like _paying for a service_ (extra child care time), and $5 was apparently a price many parents were happy to pay. The lecture's memorable summary: "A fine is a price. Once a price, always a price." Even after the fine was later removed, late pickups stayed high, because the social norm had already been replaced by a market mindset.

**2. Monetary incentives and IQ test performance (Gneezy and Rustichini, 2000, QJE).** 160 students at the University of Haifa answered IQ style questions under different payment schemes: $0 per correct answer, $0.10, $1, or $3. The point of this study, in the context of the lecture, is to test whether "more money always means better performance" (the normative, textbook prediction). The finding that made this famous is that the relationship was not simply monotonic the way a naive incentive model would predict, small payments did not straightforwardly outperform no payment, which raises interesting questions about how intrinsic motivation and monetary incentives interact rather than simply adding together.

**3. Working for yourself versus for charity (Imas, 2014).** This study used a 2x2 design: people exerted physical effort (squeezing a hand dynamometer), and the payoff either went to themselves or to charity, at either a high or low incentive level. The interesting question this design lets you answer: does _who benefits_ from your effort change how you respond to incentive size? This gets at whether prosocial motivation (wanting to help a good cause) and standard financial self-interest behave the same way as incentives get bigger, or whether they interact differently.

The overall takeaway for the course: "incentives matter" is true and useful, but real human responses to incentives can be more complicated than "more reward equals proportionally more effort," and a manager needs to think carefully about how an incentive scheme will actually be interpreted by the people responding to it.

---

## 4. Understand Markets

Every market transaction has two sides, a buyer and a seller (or equivalently, an employer and a worker in a labor market). The bargaining position of each side is shaped by three kinds of rivalry:

1. **Consumer-producer rivalry**: buyers want the lowest price possible, sellers want the highest price possible. Each side is trying to capture as much value from the transaction as it can.
2. **Consumer-consumer rivalry**: consumers compete with each other for limited goods. Think of a fixed number of Taylor Swift concert tickets, where fans are effectively bidding against each other.
3. **Producer-producer rivalry**: firms compete with each other to be the one that makes the sale, through price, quality, and product differentiation.

There is also a fourth actor worth remembering: **government**. Firms sometimes lobby government to intervene in ways that reduce competitive rivalry in their favor, for example securing status as the sole electricity supplier in a region, which removes producer-producer rivalry entirely for that firm.

### Intertemporal choices

An **intertemporal choice** is a decision where the costs and benefits do not happen at the same time, they are spread across different time periods. Since a dollar (or an hour, or an ounce of effort) today is not obviously equivalent to the same amount tomorrow, we need a framework to compare them. Two broad patterns from lecture:

1. **Immediate costs, delayed benefits.** Exercising, dieting, and studying all cost you something (effort, discomfort) right now, and the payoff (health, grades) arrives later. The behavioral challenge is forcing yourself to pay the cost now for a future reward.
2. **Immediate benefits, delayed costs.** Drinking, gambling, and eating a lot of sugar all feel good right now, and the cost (hangover, financial loss, health problems) arrives later. The behavioral challenge here is resisting the temptation of instant gratification.

### Why we discount the future

Given a choice between $1000 today and $1000 in one year, most people prefer today. This is called being impatient, and economists build this preference directly into models through **discounting**. Three reasons this preference makes sense, not just as a psychological quirk but as a rational response:

- **Impatience** itself (a genuine preference for consuming now).
- **Uncertainty about the future** (a dollar promised later might not actually arrive).
- **Option value** (money in hand today can be invested or used for other opportunities that might arise between now and later, so holding it gives you flexibility).

Lecture gives a concrete way to see this: at a 6 percent interest rate, $1000 today grows into $1060 in one year. So if someone offers you $1000 in a year instead of today, they are effectively asking you to forgo the $60 you could have earned by having the money now. This is exactly why the next section builds a formal tool, the time value of money, to make these comparisons precise instead of just intuitive.

---

## 5. Time Value of Money

This section gives you the formal math to compare cash flows that happen at different points in time, which is exactly what "discounting the future" above was gesturing at informally.

### Future Value (FV)

```
FV = PV × (1 + i)^n
```

Where PV is present value, i is the interest rate, and n is the number of time periods.

**Worked example:** $100 invested at 4 percent interest for two years.

```
FV = (1 + 0.04)^2 × $100 = $108.16
```

Two important patterns to internalize from the formula itself:

- The larger n (the further away the payoff), the smaller its value looks when brought back to today (holding PV fixed and solving backward for PV given a fixed FV).
- The larger i (the higher the interest rate, meaning the more valuable it is to have cash in hand now to invest), the smaller a future payment is worth today.

### Present Value (PV)

Rearranging the future value formula gives present value:

```
PV = FV ÷ (1 + i)^n
```

Present value is often described as "future value minus the opportunity cost of waiting," since receiving money later means giving up whatever return you could have earned by having it now.

For a whole _stream_ of future cash flows across multiple years, you just discount each one back to today separately and add them up:

```
PV = FV(1) ÷ (1+i)^1 + FV(2) ÷ (1+i)^2 + FV(3) ÷ (1+i)^3 + ... + FV(n) ÷ (1+i)^n
```

**Worked example: comparing two projects.** Project A pays $150,000 today (year 0). Project B pays $0 in year 0, $10,000 in year 1, $50,000 in year 2, and $100,000 in year 3. Assume a 3 percent annual interest rate.

```
PV(B) = $10,000 ÷ (1.03)^1 + $50,000 ÷ (1.03)^2 + $100,000 ÷ (1.03)^3
      ≈ $148,352.70
```

Since PV(A) = $150,000 is larger than PV(B) ≈ $148,352.70, Project A is the better choice even though the two projects might look similar if you just added up the raw dollar amounts ($150,000 versus $160,000 nominal). This is the entire point of time value of money: never compare raw dollar totals across different time periods, always bring them to a common point in time first.

### Net Present Value (NPV)

```
NPV = PV(benefits) − PV(costs)
```

Decision rule:

- If NPV is greater than 0, the deal creates value, take it.
- If NPV is less than 0, the deal destroys value, reject it.
- If NPV equals 0, you are exactly indifferent, the deal breaks even in present value terms.

**Worked example (simple loan to an uncle):** You lend your uncle $100, and he promises to pay you back $150 in 5 years. You could otherwise earn 10 percent interest elsewhere. Is this a good deal?

```
FV of your $100 if invested elsewhere for 5 years = (1.10)^5 × $100 ≈ $161.05
PV of the uncle's $150 offer, 5 years from now = $150 ÷ (1.10)^5 ≈ $93.18
NPV = $93.18 − $100 = −$6.86
```

Since NPV is negative, this is a bad deal: giving your uncle $100 today only gets you the equivalent of about $93.18 in today's dollars, which is less than the $100 you gave up.

**Worked example (multi period cash flows on both sides):** You lend your uncle $50 today (t=0) and another $50 one year from now (t=1). He starts paying you back $35 per year for three years, beginning three years after his _first_ loan, so payments land at t=3, t=4, and t=5. The interest rate is 3 percent.

```
PV(costs) = $50 + $50 ÷ (1.03)^1 = $98.54

PV(benefits) = $35 ÷ (1.03)^3 + $35 ÷ (1.03)^4 + $35 ÷ (1.03)^5 ≈ $93.31

NPV = $93.31 − $98.54 = −$5.23
```

Negative NPV again, so this is not a good deal either. Notice the mechanical process is exactly the same as before, discount every single cash flow back to today individually using its own specific time period, then subtract total cost PV from total benefit PV.

### Perpetuities: valuing cash flows that never end

Some assets (or promises) generate the same cash flow forever. The present value of a constant, never ending cash flow stream is remarkably simple:

```
PV (perpetuity) = CF ÷ i
```

Where CF is the constant cash flow received each period, and i is the interest rate.

**Worked example:** your uncle promises to pay you $1 a year, forever (and after he is gone, his descendants keep paying), starting from a $100 loan, at a 10 percent interest rate.

```
PV = $1 ÷ 0.10 = $10
NPV = $10 − $100 = −$90
```

A terrible deal. The lecture then flips the question: what is the _minimum_ annual payment forever that would make this a break even deal (NPV = 0)?

```
Set PV(benefits) = $100 (to match the $100 cost)
$100 = Future Payment ÷ 0.10
Future Payment = $100 × 0.10 = $10 per year, forever
```

So your uncle would need to promise $10 a year forever, not $1, for this to be a fair deal at a 10 percent interest rate. This is a very useful sanity check pattern: perpetuity value is just cash flow divided by interest rate, so you can solve for whichever variable you're missing.

### A useful tangent: the power of exponential growth

Lecture includes a classic thought experiment to build intuition for how fast exponential (doubling) growth compounds, which is directly relevant to why interest rates and growth rates matter so much over long horizons.

Choice A: take $1 billion today. Choice B: take 1 cent on the first square of a chessboard, and double it on every subsequent square, for all 64 squares.

The total under Choice B is:

```
1 + 2 + 4 + ... + 2^63 = 2^64 − 1 cents ≈ $184,467,440,737,095,516.15
```

That is roughly $184 quadrillion, absolutely dwarfing $1 billion. The lesson: doubling (or any compounding growth process) looks slow and unremarkable early on, then becomes almost incomprehensibly large. This is exactly the same mechanism that makes compound interest so powerful over long time horizons, and it is why even small differences in interest rate or growth rate assumptions make a huge difference decades out.

### Valuing a firm with growing profits (the Gordon growth idea)

If a firm currently earns profit π0, pays no dividends, and its profit is expected to grow at a constant rate g forever (assuming g is less than i), the present value of the entire firm is:

```
PV(firm) = π0 × (1 + i) ÷ (i − g)
```

**Where this formula comes from (worked derivation):** Write out the value as an infinite sum of each future year's profit, discounted back:

```
PV = π0(1+g)/(1+i) + π0(1+g)^2/(1+i)^2 + π0(1+g)^3/(1+i)^3 + ...
```

Define r = (1+g) ÷ (1+i) as a common ratio. This is now a geometric series:

```
1 + r + r^2 + r^3 + ... = 1 ÷ (1 − r)
```

So the whole sum becomes:

```
PV = π0 × ( 1 ÷ (1 − r) )
```

Substituting r back in and simplifying the denominator:

```
1 − (1+g)/(1+i) = [(1+i) − (1+g)] ÷ (1+i) = (i − g) ÷ (1+i)
```

Flipping that fraction to finish simplifying:

```
PV = π0 × ( (1+i) ÷ (i − g) )
```

Which is exactly the formula above. The key mechanical trick worth remembering here, beyond finance specifically, is that "growing perpetuity" problems always reduce to a geometric series, and geometric series always collapse to that same 1 ÷ (1 − r) shape.

---

## 6. Use Marginal Analysis

This is arguably the single most important tool from this lecture, and it reappears constantly for the rest of the course (cost minimization, profit maximization under any market structure, all of it reduces to this same logic).

### The setup

Let Q be the manager's control variable (how much of something to do, produce, buy, and so on).

- **Total benefit**: B(Q)
- **Total cost**: C(Q)
- **Net benefit**: N(Q) = B(Q) − C(Q), also written as Π = B(Q) − C(Q)

### Marginal quantities

- **Marginal benefit, MB(Q)**: the change in total benefit from a small change in Q.
- **Marginal cost, MC(Q)**: the change in total cost from a small change in Q.
- **Marginal net benefit, MNB(Q)**: MB(Q) − MC(Q).

If the control variable is continuous (infinitely divisible), then marginal values are just the **slope** of the corresponding total curve at a given point, meaning the first derivative from calculus. Slope of the total benefit curve at some Q equals MB at that Q, slope of the total cost curve equals MC, and slope of the net benefit curve equals MNB.

### The core decision rule

> To maximize net benefit, increase the control variable up to the point where marginal benefit equals marginal cost (MB = MC). At that point, marginal net benefit is zero, meaning nothing more can be gained by changing the variable further.

Why does this work? Think about it directly in terms of the two possible mistakes:

- If **MB > MC** at your current Q, you should do more. Each additional unit is bringing in more benefit than it costs, so stopping here leaves money on the table.
- If **MB < MC**, you should do less. The last unit you did cost you more than it was worth.
- Only when **MB = MC** are you doing exactly the right amount, any more or less would make you worse off.

**Worked intuition (Lamar's lemonade, one more glass at a time):** If making one more glass costs $1 (marginal cost) and it sells for $3 (marginal benefit), making it adds $2 of profit, clearly worth doing (MB > MC). But suppose costs rise as you scale up (this is realistic, since ingredients might get scarcer or you get more tired), so eventually the next glass costs $1.50 and only sells for $2. That is still MB > MC (barely), so it is still worth making. The manager keeps making more glasses only up until the point where the next glass would cost exactly what it sells for. Past that point, MC would exceed MB and making more would actually reduce profit.

**Fully worked numeric example:** Given B(Q) = 250Q − 4Q^2 and C(Q) = Q^2, find the profit maximizing Q.

Step 1: take the derivative of each to get marginal benefit and marginal cost.

```
MB(Q) = 250 − 8Q
MC(Q) = 2Q
```

Step 2: set MB(Q) = MC(Q) and solve for Q, since that is where marginal net benefit equals zero.

```
250 − 8Q = 2Q
250 = 10Q
Q = 25
```

So the manager should choose Q = 25 to maximize net benefit given these specific benefit and cost functions.

### Related vocabulary worth memorizing

- **Incremental revenue**: the additional revenue that results from a specific yes-or-no decision (not a "per unit" marginal concept necessarily, but the total change from making that one decision).
- **Incremental cost**: the additional cost from that same yes-or-no decision.
- **"Thumbs up" decision**: take the action whenever MB > MC.
- **"Thumbs down" decision**: reject the action whenever MB < MC.

---

## 7. Make Data Driven Decisions

Good managerial decisions rely on actually knowing things like the shape of demand for your product, not just gut instinct. Lecture lists several ways to get that information: published data and papers, econometric modeling, hiring a consultant, or (only half jokingly) asking an AI assistant. The main statistical tool introduced here is **regression analysis**.

### The regression model

The true (unobservable, theoretical) relationship is assumed to look like:

```
Y = a + bX + e
```

Where:

- a is the true, unknown population intercept
- b is the true, unknown population slope (this is usually the number you actually care about, since it tells you how much Y changes when X changes)
- e is a random error term with mean zero and some standard deviation, representing everything affecting Y that is not captured by X

Since you can never observe the whole population, you estimate a and b from a sample using **Ordinary Least Squares (OLS) regression**, producing the fitted line:

```
Ŷ = â + b̂X
```

The little hats mean "our best estimate of," not the true value. â and b̂ are chosen specifically to minimize the sum of squared differences (errors) between the fitted line and the actual data points, hence "least squares."

An important nuance from lecture: b̂ is not the true b, it is a prediction of how Y tends to move when X changes, based on a limited sample. This distinction matters because a sample based estimate will always have some noise or uncertainty compared to the true relationship you would get if you had every data point in existence.

Lecture also mentions two extensions of the same basic idea, useful in different situations:

- **Log-linear regression**: ln(Y) = a + b·ln(X) + e. You transform both variables into their logarithms before running the regression. This is especially useful in economics because the slope b in a log-log regression is directly interpretable as an elasticity (percent change in Y for a percent change in X), which is a concept you will use heavily later in the course.
- **Multiple regression**: Y = a + b1X1 + b2X2 + ... + bkXk + e. This lets you control for more than one explanatory variable at once, which matters a lot for the next topic: correlation versus causation.

### Correlation is not causation

This is presented through a deliberately provocative example. Suppose you have data on every person's age at death and how many glasses of wine they drank per day, and a regression shows that each extra glass of wine per day is associated with living 2.4 years longer. Does drinking wine cause you to live longer?

**No.** And working through exactly why is the real lesson here.

**Omitted variable bias**: there may be a third factor that affects both wine consumption and lifespan, making them move together in the data even though neither one is directly causing the other. Two explanations given in lecture:

- People who drink more wine tend to be wealthier, and wealthier people tend to have better healthcare, which is the actual thing extending their lives, not the wine itself.
- Wine tends to be consumed more in warmer climates, and people in warmer climates might get more vitamin D or other lifestyle benefits that independently improve health.

Even if you had data on every _observable_ variable (wealth, climate, and so on) and controlled for all of them in a multiple regression, lecture points out you would still not be safe, because of a second, sneakier problem:

**Selection effects**: people self select into behaviors based on _unobservable_ traits that you cannot put a number on and control for. Example given: people who enjoy taking more risks might be more likely to drink hard liquor rather than wine, and those same risk loving people are independently more likely to die younger for unrelated risky-behavior reasons. Risk tolerance is not something you can easily measure and add as a control variable, so it stays hidden in the error term and can create a spurious relationship between what you can observe (wine versus liquor) and the outcome (lifespan).

Another selection effect example from lecture: an unemployment job training program might appear to boost employment, but if the people who chose to enroll were already more motivated to find work in the first place, the program itself might be doing nothing, you would just be observing that motivated people succeed more, with or without the program.

Economists care enormously about this distinction because policy decisions require genuinely _causal_ answers (does the program work), not just correlational ones (do people who take the program tend to do better anyway).

### Randomization as the solution

The cleanest way to eliminate selection effects entirely is **randomization**, meaning running a controlled experiment where assignment to treatment is determined by pure chance rather than by personal choice or traits.

**Worked example:** suppose there are 10,000 unemployed people, and you want to know if a job training program actually causes higher employment. Instead of letting people opt in (which reintroduces selection effects, since more motivated people would be more likely to opt in), you flip a coin for each person: heads means they join the program (treatment group), tails means they do not (control group).

Because assignment is random, both **observed** traits (education, age) and **unobserved** traits (motivation, risk tolerance, anything else you could never measure) end up, on average, equally distributed between the two groups. Since the two groups start out statistically identical in every way except whether they got the program, any difference in employment outcomes between the groups afterward can be attributed to the program itself (assuming everyone actually follows their assigned group, referred to as "full compliance"). This is exactly why randomized controlled trials (RCTs) are considered the gold standard for establishing causation in economics and other sciences.

---

## Quiz Question, worked through

> Maria quits her job paying $60,000 a year to open a bakery. In her first year, the bakery brings in $150,000 in revenue, and she pays $100,000 for ingredients, rent, and equipment. What is her economic profit in the first year? A. $50,000 B. $90,000 C. −$10,000 D. $10,000

This question is really testing whether you remember the difference between accounting profit and economic profit from section 2.

**Accounting profit** only subtracts the explicit costs she actually paid cash for:

```
Accounting profit = $150,000 − $100,000 = $50,000
```

That $50,000 is answer A, and it is a real number, it is just the wrong number for this question, because it ignores her opportunity cost entirely.

**Economic profit** also subtracts the implicit cost of what she gave up, which here is the $60,000 salary she walked away from to run the bakery:

```
Economic profit = $150,000 − $100,000 − $60,000 = −$10,000
```

So the answer is **C, −$10,000**. The bakery actually made her worse off in year one compared to her next best alternative (staying at her old job), even though it looked profitable ($50,000 in the black) by ordinary accounting standards. This is exactly the gap between accounting profit and economic profit that section 2 spent so much time on, and it is a great one sentence summary of why the distinction matters in the real world: a business can look profitable on paper while actually representing a worse choice than the option you gave up.

---

## Quick Reference Summary

- **Profit**: Π = TR − TC. Economic profit also subtracts implicit (opportunity) costs, not just explicit ones.
- **Opportunity cost**: value of your best foregone alternative. Ignore sunk costs and costs identical across all options.
- **Five Forces**: entry, supplier power, buyer power, rivalry, substitutes and complements, all describe threats to _sustained_ profit.
- **Incentives**: people act when MB exceeds MC for them personally. Watch for perverse incentives, where people optimize the letter of a rule rather than its intent.
- **Markets**: shaped by consumer-producer, consumer-consumer, and producer-producer rivalry, plus possible government intervention.
- **Time value of money**: FV = PV × (1+i)^n. NPV = PV(benefits) − PV(costs). Take a deal only if NPV is greater than 0. Perpetuity PV = CF ÷ i.
- **Marginal analysis**: increase your control variable until MB = MC. That is the profit maximizing point.
- **Data driven decisions**: regression estimates relationships, but correlation is not causation, watch for omitted variable bias and selection effects. Randomization is the cleanest fix.