# Beer Game - Complete Guide

##  Quick Reference Card

### Your Goal
**Minimize your total cost = ($1 × Inventory) + ($2 × Backlog)**

### The Three Steps (Every Day)
1. **Move Pipeline** - Advance inventory through delivery stages
2. **Prepare Order** - Decide quantity when you have Kanban card
3. **Deliver Beer** - Fill customer orders, receive supplier deliveries

---

##  Game Overview

### Supply Chain Structure
```
Consumer → Retailer → Wholesaler → Distributor → Brewery
         ←  3 days  ←   3 days   ←   3 days   ← 2 days
```

- **Total simulation**: 40 days
- **Expected consumer demand**: 4 kegs initially, likely to increase
- **Your role**: One of four positions in the chain
- **Team size**: 9-10 students (2 per role + 1 leader as consumer)

### Lead Times
- **Brewery**: 2 days to produce
- **Distributor**: 3 days to deliver
- **Wholesaler**: 3 days to deliver
- **Retailer**: 3 days to deliver

---

##  Detailed Gameplay

### Step 1: Move the Pipeline

**What happens:**
- All inventory in transit moves one stage closer to warehouse
- Leftmost stage MUST be empty after this step
- All four parties do this simultaneously
- No delivery to customer yet

**Visual:**
```
Stage 1 → Stage 2 → Warehouse
(empty)  (moves→)  (receives)
```

**Important:**
- Record what arrives at your warehouse in the "Received" column
- This is what you'll use to fill orders in Step 3

---

### Step 2: Prepare Your Order

**Critical Rules:**
- ✅ You MUST have the Kanban card to make this decision
- ✅ Record your order quantity immediately
- ✅ Pass Kanban card to next person downstream
- ❌ You do NOT know what next period's demand will be
- ❌ Do NOT collude with other supply chain members

**Order Flow:**
1. Brewer decides production quantity → passes Kanban to Distributor
2. Distributor decides order quantity → passes Kanban to Wholesaler
3. Wholesaler decides order quantity → passes Kanban to Retailer
4. Retailer decides order quantity → passes Kanban to Consumer
5. Consumer receives demand from instructor → returns Kanban to Brewer

**What You Know:**
- ✅ Your current inventory
- ✅ Your current backlog
- ✅ What you just received (Step 1)
- ✅ Historical orders from your customer
- ❌ Future demand
- ❌ What's happening elsewhere in the chain

---

### Step 3: Deliver Beer

**Calculation Process:**

#### 3a. Calculate Total Number Required
```
Total Required = New Order + Existing Backlog
```
**Example:** Customer orders 10, you owe 5 backlog → You need 15 total

#### 3b. Determine Actual Delivery
```
Actual Delivery = MIN(Total Required, Warehouse Inventory)
```

#### 3c. Update Backlog
```
New Backlog = Total Required - Actual Delivery
```

#### 3d. Update Inventory
```
New Inventory = Warehouse Inventory - Actual Delivery
```

### Delivery Examples

**Example 1: Sufficient Inventory**
- New order: 10 kegs
- Current backlog: 0
- Warehouse inventory: 12 kegs
- **Deliver**: 10 kegs
- **New inventory**: 2 kegs
- **New backlog**: 0

**Example 2: Insufficient Inventory (No Prior Backlog)**
- New order: 10 kegs
- Current backlog: 0
- Warehouse inventory: 3 kegs
- **Deliver**: 3 kegs (all you have)
- **New inventory**: 0
- **New backlog**: 7 kegs

**Example 3: Insufficient Inventory (With Prior Backlog)**
- New order: 10 kegs
- Current backlog: 5 kegs
- Warehouse inventory: 3 kegs
- **Total required**: 15 kegs
- **Deliver**: 3 kegs (all you have)
- **New inventory**: 0
- **New backlog**: 12 kegs

---

##  Cost Calculations

### Cost Formula
```
Daily Cost = ($1 × Inventory) + ($2 × Backlog)
```

### Why Backlog Costs More
- Backlog represents unfilled customer orders
- Creates customer dissatisfaction
- More expensive to rush/expedite
- Costs 2× as much as holding inventory

### Can You Have Both?
**NO!** You should never have both inventory and backlog simultaneously.
- If you have inventory, you can fill the backlog
- If you have backlog, your inventory must be zero

---

##  Data Entry Form

### Columns to Track

| Day | Received | Order Quantity | Demand | Delivery | Backlog | Inventory | Cost |
|-----|----------|----------------|---------|----------|---------|-----------|------|
| 1   | ...      | ...            | ...     | ...      | ...     | ...       | ...  |

**Step 1**: Record "Received" (what arrives at warehouse)
**Step 2**: Record "Order Quantity" (your decision)
**Step 3**: Record "Demand" (what customer ordered from you)
**Step 3**: Record "Delivery" (what you actually shipped)
**Step 3**: Calculate and record "Backlog"
**Step 3**: Calculate and record "Inventory"
**Step 3**: Calculate and record "Cost"

---

##  Kanban Card System

### What is Kanban?
- A card that signals authorization to produce/order
- Ensures you don't know future demand when deciding
- Circulates through the supply chain each day

### Kanban Flow
```
Brewer → Distributor → Wholesaler → Retailer → Consumer → (back to Brewer)
```

### Rules
- Only decide when YOU have the card
- Write decision immediately
- Pass card immediately after deciding
- Leader returns card to Brewer after Step 2

---

##  Strategic Guidance

### Common Mistakes to Avoid

#### 1. **Panic Ordering (The Bullwhip Effect)**
- ❌ Seeing a shortage and massively over-ordering
- ❌ Reacting emotionally to backlog
- ✅ Remember lead times - orders take days to arrive
- ✅ Consider what you already have in the pipeline

#### 2. **Ignoring Lead Times**
- ❌ Forgetting your orders won't arrive for 2-3 days
- ✅ Think ahead about pipeline inventory
- ✅ Account for in-transit goods in your calculations

#### 3. **Not Tracking Pipeline**
- ❌ Only looking at warehouse inventory
- ✅ Know what's coming in the next few days
- ✅ Consider total inventory position

#### 4. **Poor Communication**
- ❌ Not discussing strategy with your partner
- ✅ Work as a team with your position partner
- ✅ Observe patterns in customer orders

---

### Strategic Approaches

#### Conservative Strategy
**Goal:** Avoid backlog at all costs
- Order slightly above recent demand
- Build small safety stock
- Accept higher inventory costs
- **Risk:** High inventory costs if demand doesn't increase

#### Balanced Strategy
**Goal:** Minimize total cost
- Match orders to smooth demand trends
- Maintain minimal safety stock (2-3 units)
- Accept small temporary backlogs
- **Risk:** Requires accurate demand forecasting

#### Aggressive Strategy
**Goal:** Minimize inventory
- Order exactly to demand
- No safety stock
- **Risk:** Backlogs cost 2× inventory, very risky

---

### Decision-Making Framework

#### Questions to Ask Each Turn

1. **What's my current position?**
   - Inventory: ___
   - Backlog: ___
   - Pipeline (in-transit): ___

2. **What's the demand trend?**
   - Last 3 orders: ___, ___, ___
   - Stable? Increasing? Decreasing?

3. **What's arriving soon?**
   - Next period: ___
   - Period after: ___

4. **What's my total inventory position?**
   ```
   Total Position = Warehouse + Pipeline - Backlog
   ```

5. **What should I order?**
   ```
   Order = Expected Demand + Desired Safety Stock - Total Position
   ```

---

### Sample Order Decision Process

**Scenario:**
- Current inventory: 8 kegs
- Current backlog: 0
- Pipeline: 6 kegs coming in 2 days, 4 kegs in 3 days
- Recent customer orders: 4, 4, 5, 6, 7

**Analysis:**
- Demand is increasing (4→7 over 5 days)
- Total position = 8 + 6 + 4 - 0 = 18 kegs
- Expected demand next 3 days ≈ 7-8 kegs/day
- Need ≈ 24 kegs for 3 days

**Decision:**
- Total position (18) < Expected need (24)
- Order: 24 - 18 = 6 kegs
- Includes small safety buffer for increasing trend

---

##  Chip Representation System

### Chip Values
- 🔵 Blue chip = 8 kegs
- 🔴 Red chip = 4 kegs
- ⚪ White chip = 1 keg
- 📎 Paper clip = 0 kegs (placeholder)

### Making Change
- You CAN exchange chips for lower denominations
- Example: 1 blue (8) = 2 red (4+4)
- Example: 1 red (4) = 4 white (1+1+1+1)

### Using Paper Clips
- Use when delivering 0 kegs
- Use when warehouse is empty (different from pipeline stage)
- Shows intentional zero vs. empty space

---

##  Critical Rules & Restrictions

### Absolute Rules
1. ✅ **Only order when you have the Kanban card**
2. ✅ **Record your decision immediately**
3. ✅ **All parties move pipeline simultaneously in Step 1**
4. ✅ **Leftmost stage must be empty after Step 1**
5. ✅ **Backlog must be filled and accumulates**

### Prohibitions
1. ❌ **NO collusion** with other supply chain members
2. ❌ **NO advance information** about future demand
3. ❌ **Leader does NOT disclose** future consumer demand
4. ❌ **Never have both** inventory and backlog simultaneously

### Leader Responsibilities
- Call each step clearly
- Ensure forms are completed before next day
- Do NOT decide order quantity yourself
- Do NOT show future demand to players
- Return Kanban to Brewer after Step 2
- Announce beginning of next day after returning Kanban

---

##  What to Observe

### During the Game
- How does your inventory fluctuate?
- What happens to backlogs over time?
- Do you see patterns forming?
- How long does it take to recover from a spike?
- What's happening at other positions?

### The Bullwhip Effect
**Watch for:**
- Small demand changes at consumer level
- Larger order swings at retailer level
- Even larger swings at wholesaler level
- Massive swings at brewery level

**Why it happens:**
- Information delays (lead times)
- Lack of supply chain visibility
- Independent decision-making
- Panic ordering when seeing shortages
- Over-correction behaviors

---

##  Quick Math Reference

### Total Required Calculation
```
Total Required = New Customer Order + Your Current Backlog
```

### Delivery Calculation
```
Actual Delivery = MIN(Total Required, Warehouse Inventory)
```

### New Backlog Calculation
```
New Backlog = MAX(0, Total Required - Actual Delivery)
```

### New Inventory Calculation
```
New Inventory = MAX(0, Warehouse Inventory - Actual Delivery)
```

### Cost Calculation
```
Cost = (Inventory × $1) + (Backlog × $2)
```

### Total Inventory Position (for ordering decisions)
```
Total Position = Warehouse + Pipeline - Backlog
```

---

##  Pro Tips
### Before the Game
1. Review all calculations until comfortable
2. Discuss strategy with your partner
3. Agree on decision-making approach
4. Set up your data form clearly

### During Each Turn
1. Track your pipeline carefully
2. Look for demand trends, not just last order
3. Don't panic - remember lead times
4. Communicate with your partner
5. Think 2-3 days ahead

### Common Pitfalls
- Over-reacting to one unusual order
- Forgetting what's in your pipeline
- Not accounting for lead times
- Making decisions too conservatively early on
- Panic ordering when you see backlog building

### Recovery Strategies
- If you build backlog: Order extra, but not crazy extra
- If you build inventory: Reduce orders temporarily
- Always consider what's already in pipeline
- Smooth out your orders rather than wild swings

---

##  Learning Objectives

### What This Game Teaches

1. **Supply Chain Dynamics**
   - How delays amplify upstream
   - Information flow vs. product flow
   - Interdependencies in systems

2. **Bullwhip Effect**
   - Why small demand changes create huge supply swings
   - Role of forecasting and information sharing
   - Impact of decentralized decision-making

3. **Inventory Management**
   - Trade-offs between holding costs and stockouts
   - Safety stock decisions
   - Lead time management

4. **Systems Thinking**
   - Local optimization vs. system optimization
   - Feedback loops and delays
   - Unintended consequences

---

##  Post-Game Reflection Questions

### For Class Discussion

1. What happened to your inventory/backlog over time?
2. What was your peak backlog? When did it occur?
3. What ordering strategy did you use?
4. When did you realize demand was changing?
5. How did you respond to shortages?
6. What would you do differently?
7. How could the supply chain coordinate better?
8. What real-world parallels do you see?

### Key Insights to Watch For
- The amplification of orders upstream
- Time it takes for system to stabilize
- Difference between local and system optimization
- Value of information sharing
- Impact of lead times on decision-making

---

##  Related Concepts

### Operations Management Topics
- [[Supply Chain Management]]
- [[Inventory Management]]
- [[Bullwhip Effect]]
- [[Systems Thinking]]
- [[Lean Manufacturing]]
- [[Kanban Systems]]
- [[Demand Forecasting]]
- [[Safety Stock]]

### Real-World Applications
- Retail supply chains (seasonal products)
- Manufacturing (automotive, electronics)
- Pandemic supply chain disruptions
- Just-in-time vs. Just-in-case inventory
- Information sharing initiatives (CPFR, VMI)

---

##  Additional Resources
### If You Want to Learn More
- Original MIT Beer Game development (1960s)
- Peter Senge's "The Fifth Discipline"
- Supply chain coordination strategies
- Information technology in supply chain management
- Vendor Managed Inventory (VMI) systems

---

##  Pre-Game Checklist

Before starting:
- [ ] Understand all three steps
- [ ] Know the cost formula
- [ ] Can calculate deliveries correctly
- [ ] Understand Kanban card flow
- [ ] Know your role's lead time
- [ ] Have discussed strategy with partner
- [ ] Data entry form is ready
- [ ] Chips and materials organized

During game:
- [ ] Track pipeline inventory
- [ ] Record all decisions immediately
- [ ] Calculate costs each round
- [ ] Look for demand patterns
- [ ] Communicate with partner
- [ ] Stay calm and think ahead

---

##  Summary: Keys to Success

1. **Understand the mechanics** - Know the rules cold
2. **Track your pipeline** - Don't just look at warehouse
3. **Identify trends** - Don't react to single data points
4. **Account for lead times** - Orders take days to arrive
5. **Stay calm** - Panic ordering makes it worse
6. **Work with your partner** - Two heads are better than one
7. **Think ahead** - Where will you be in 2-3 days?
8. **Learn from it** - The game is about insight, not winning
