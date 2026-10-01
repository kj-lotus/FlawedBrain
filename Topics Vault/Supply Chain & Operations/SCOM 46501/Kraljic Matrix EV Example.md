---
topic: "Supply Chain & Operations"
related-topics: [Business Strategy & Competitive Advantage]
source-class: "SCOM 46501"
source-semester: "Fall 2027"
created: 2026-10-01
tags:
  - topic/ops
  - topic/strategy
  - class/SCOM-46501
  - sourcing
  - kraljic
  - category-management
---

# Kraljic Matrix: EV Example

> [!summary] One line version
> The Kraljic Matrix sorts purchased items by **profit impact** and **supply risk**, then gives each of the 4 groups its own sourcing strategy. The point is to spend procurement effort where it matters most.

## Background

- Created by **Peter Kraljic** in the Harvard Business Review article "Purchasing Must Become Supply Management" (1983)
- It was one of the first tools to treat purchasing as **strategic** instead of just clerical buying
- Still the most common **portfolio model** in [[Category Management]]

## The two axes

**Profit impact** (vertical axis): how much the item affects cost, quality, or the value of the final product
- Share of total spend
- Effect on product quality or performance
- Volume purchased
- Impact on business growth

**Supply risk** (horizontal axis): how hard or risky the item is to get
- Number of available suppliers
- Supplier market concentration (monopoly or oligopoly)
- Switching costs and qualification time
- Substitute availability
- Geopolitical and logistics risk
- Storage limits (shelf life, hazmat)

> [!tip] How to actually place an item
> Score each item 1 to 5 on several factors for each axis, weight the factors, and average them. Anything above the midpoint goes into the "high" side. This makes the placement defensible instead of a gut call, which is a good thing to mention on a test or case write up.

## The 4 quadrants at a glance

| | **Low supply risk** | **High supply risk** |
|---|---|---|
| **High profit impact** | **Leverage** (exploit buying power) | **Strategic** (partner and secure) |
| **Low profit impact** | **Non critical** (simplify and automate) | **Bottleneck** (secure continuity) |

## Strategic items

High impact, high risk

### EV examples
- **Battery cells**: biggest single cost in the car, made by a few global makers (CATL, LG, Panasonic, BYD)
- **Cathode raw materials** (lithium, nickel, cobalt): volatile prices, mining and refining concentrated in a few countries
- **Silicon carbide power semiconductors** for the inverter: drive efficiency and range, very few suppliers
- **Rare earth permanent magnets** (NdFeB) for the drive motor: China controls most processing

### Supply chain setup
- **Supplier base:** 2 or 3 deeply qualified partners, never single sourced
- **Relationship:** strategic partnerships, joint ventures, or [[Vertical Integration & Diversification|Vertical Integration]]
	- GM and LG: Ultium Cells
	- Ford and SK On: BlueOval SK
	- Tesla building its own 4680 cells
- **Contracts:** long term agreements (5 to 10 years) with volume commitments and **index based pricing** tied to commodity markets so risk is shared
- **Upstream control:** offtake agreements or equity stakes in mines and refiners
- **Geography:** regionalize near assembly plants to cut risk and qualify for IRA tax credits in the US
- **Inventory and logistics:** moderate buffer, hazmat carriers for batteries
- **Risk management:** multi tier supplier mapping, geopolitical monitoring, battery recycling, backup chemistries like LFP that avoid cobalt and nickel
- **KPIs:** total cost of ownership, supply assurance, joint innovation, quality

## Leverage items

High impact, low risk

### EV examples
- Steel and aluminum body panels and stampings
- Tires
- Seats
- Glass (windshield and windows)
- Wiring harnesses
- Interior trim and plastics

### Supply chain setup
- **Supplier base:** many qualified suppliers kept in competition
- **Relationship:** arm's length and transactional
- **Contracts:** 1 to 3 years, rebid often using RFQs and [[Reverse Auctions]], split volume (for example 70 and 30) to keep suppliers competing
- **Consolidation:** pool demand across vehicle platforms and standardize specs so more suppliers can bid
- **Inventory and logistics:** **just in time (JIT)** and **just in sequence (JIS)**, with suppliers in parks near the plant
- **Risk management:** low, but watch steel and aluminum prices and hedge if needed
- **KPIs:** unit price, savings achieved, on time delivery, defect rate

## Bottleneck items

Low impact, high risk

### EV examples
- **Microcontroller chips** in control modules (the 2021 chip shortage)
- High voltage connectors and fuses
- Specialized sensors (battery temperature, current sensors)
- Thermal interface materials and specialty battery coolant
- Charge port assemblies with a single qualified supplier

### Supply chain setup
- **Supplier base:** usually one source exists, so qualify a backup even at higher cost
- **Relationship:** be a "customer of choice" by paying on time and sharing forecasts early
- **Contracts:** capacity guarantees, even at a premium. Some automakers now buy directly from chip foundries
- **Inventory:** break the JIT rule and hold **weeks or months of safety stock**. Cheap to hold compared to a plant shutdown
- **Redesign:** engineering and procurement swap custom parts for standard ones to move the item out of this quadrant
- **Visibility:** map down to tier 2 and tier 3, since the real bottleneck is often hidden (like the wafer fab behind a chip)
- **KPIs:** supply continuity, days of inventory on hand, number of qualified sources, lead time

## Non critical items

Low impact, low risk

### EV examples
- Fasteners (bolts, screws, clips)
- Floor mats
- Wiper blades
- Cabin air filters
- Cup holders
- Labels and packaging

### Supply chain setup
- **Supplier base:** consolidate to a few distributors covering hundreds of items
- **Relationship:** minimal, routine buying
- **Contracts:** blanket purchase orders, catalogs, e procurement with automatic reorders, purchasing cards
- **Inventory:** **vendor managed inventory (VMI)** or kanban bins
- **Standardization:** cut part number variety (same bolt across models)
- **KPIs:** transaction cost per order, number of POs processed, fill rate

## Summary table

| Quadrant | Suppliers | Contract | Inventory | Main focus | Procurement effort |
|---|---|---|---|---|---|
| Strategic | 2 to 3 partners | Long term, index pricing | Moderate buffer | Partnership and security | Very high |
| Leverage | Many, competing | Short term, auctions | JIT and JIS | Lowest cost | High |
| Bottleneck | 1 to 2, add backups | Capacity guarantees | High safety stock | Continuity | Medium |
| Non critical | Few distributors | Blanket POs, catalogs | VMI and kanban | Low admin cost | Very low |

## Extra notes worth knowing

### Items move between quadrants
The matrix is a snapshot, not permanent. Re-run it every year or after a big market change.
- **Microcontrollers** jumped from non critical to bottleneck almost overnight in 2021
- **Battery cells** may slide toward leverage as more cell makers come online
- **Lithium** shifted in risk as prices spiked in 2022 and then crashed
- A company can also **move items on purpose**: redesign a bottleneck part into non critical, or develop new suppliers to turn a strategic item into leverage

### The 80 and 20 pattern
- Non critical items are usually **most of the item count but a small share of spend**
- Strategic and leverage items are **a small number of items but most of the spend**
- This is why automating non critical buying frees up people for strategic work
- Pairs well with an [[ABC Analysis]] of spend

### The supplier's view matters too
Kraljic only looks at the **buyer's** side. The **Supplier Preferencing Model** (Steele and Court) looks at how the supplier sees you, based on how attractive your account is and how much it's worth to them.
- If an item is strategic for you but **you're a small "nuisance" account** for the supplier, you have very little power
- This explains why automakers got cut off from chips in 2021: they were a small and demanding share of chipmakers' revenue compared to phone and PC makers

> [!warning] Power position check
> Before choosing a strategy, ask who holds the power. Leverage tactics like reverse auctions will backfire on a strategic supplier that does not need your business.

### Common criticisms
- Placement can be **subjective** if you skip the scoring step
- Only **two dimensions**, so it ignores things like sustainability, innovation potential, and ethics
- Ignores the **supplier's perspective** (see above)
- Treats items as **independent** even though a supplier may sell you items in several quadrants
- Still useful as a **starting point**, not a final answer

### Connections to other course topics
- **[[Supplier Relationship Management]]**: strategic items get deep collaboration, non critical get almost none
- **[[Vertical Integration & Diversification|Vertical Integration]]**: a make or buy option mainly for strategic items
- **[[Global Sourcing]]**: works well for leverage items, risky for strategic and bottleneck ones
- **[[Reverse Auctions]]**: fit leverage items, wrong tool for strategic ones
- **[[Supply Contracts]]**: contract length and pricing type change by quadrant
- **[[Procure to Pay]]**: non critical items should run through an automated P2P process
- **[[Total Cost of Ownership]]**: the right lens for strategic items, where unit price alone misleads

## Exam tips

> [!tip] What graders usually look for
> 1. Name **both axes** correctly (profit impact and supply risk)
> 2. Give a **concrete example** for each quadrant
> 3. Match each quadrant with its **strategy** (partner, exploit, secure, simplify)
> 4. Mention that items **can move** between quadrants
> 5. Bonus: bring up the **supplier's view** or a real event like the 2021 chip shortage

**Memory trick:** "**S**ecure the **B**ottleneck, **P**artner on **S**trategic, **E**xploit **L**everage, **S**implify **N**on critical"

## Common mistakes
- Mixing up **bottleneck** and **strategic**: both are high risk, but bottleneck items are **cheap**
- Mixing up **leverage** and **non critical**: both are low risk, but leverage items are **big spend**
- Assuming high spend always means strategic. Spend alone puts an item in leverage unless supply is also risky

---

## Related Notes

- [[Whirlpool Global Procurement Pre Class Quiz Notes]]
- [[Apple Supply Chain in class - SCOM 465]]
- [[Supply Chain 1]]
- [[Bullwhip Effect]]
- [[Discounts]]
- [[Types of Costs]]
- [[Porter 5 forces - MIS 382]]
- [[Vertical Integration & Diversification]]
- [[Chapter 6 - Differentiation, Cost Leadership]]
