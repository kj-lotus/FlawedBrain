## The Big Picture

Whirlpool wants global scale and common procurement practices, but regional businesses still own their own P&L. The consulting problem is figuring out how to fairly compare procurement performance across regions without just assuming "lower price means better buying."

Price differences can come from product design, volume, geography, facility choices, or operating performance, not just negotiation skill. The real goal is not to explain price for its own sake, it is to find the cost drivers Whirlpool can actually influence through sourcing, specification, process changes, or supplier management.

Key idea to remember for the quiz: quoted price is not the same thing as supplier economics. A low price could hide a real cost disadvantage, and a high price could be justified by design or volume differences.

## The Three Cost Modeling Approaches

Whirlpool cannot use one model for every purchase. The model has to match the complexity of the item.

**Macro / trend modeling** is for raw materials like steel, resin, and foam. These prices are driven by external supply and demand, currency, and market conditions, so you track the market rather than build a bottoms up cost model.

**Bottoms up (should cost) modeling** is for simple transformations like stamping, injection molding, and packaging. The production process can be broken down into material economics and conversion economics, so you can rebuild the cost from scratch.

**Parametric modeling** is for engineered subsystems like compressors, motors, and wiring harnesses. You can observe functionality and performance, but the internal design is too complex to model part by part, so you build a statistical price model based on functional variables instead.

Think of it as a progression: market driven, then process decomposable, then engineered bundle.

## The Driver Framework (Design, Facility, Geography, Operations)

Use this framework to classify what is actually causing a cost difference.

**Design**: product specifications, functionality, product line complexity.

**Facility**: scale, equipment or process technology, automation and tooling.

**Geography**: wage rates, transportation, duties, taxes, currency.

**Operations**: productivity, utilization, scrap and rejection rates.

For the quiz, be ready to sort at least three plastic part drivers and three compressor drivers into these four buckets, and to explain a driver that could arguably fit more than one bucket.

## Plastic Parts: Bottoms Up / Should Cost Analysis

This is the simpler, more transparent case, so it gets worked first. The goal is to open a supplier quote into its components: material, labor, machine, and tooling.

Material economics: part weight multiplied by resin price gets you to the "good material" cost. Anything above that is a premium or scrap allowance you need to explain.

Labor economics: wage rate and the indirect to direct labor ratio combine to give you labor cost per part.

Machine economics: press size, hourly machine rate, and cycle time combine to determine production cost per part.

Tooling economics: parts per mold (cavities) affects output per cycle, and tooling cost has to be amortized over annual volume, so if two suppliers have different annual volumes you cannot compare tooling cost per part directly without adjusting for that.

Supplier scale: a larger supplier may get better resin purchasing economics, which shows up as a real cost advantage rather than just a negotiating trick.

The worked example in the case is the Plinth (part number 783-9488). For the quiz, know the general structure of that calculation even if you do not remember exact numbers:

Material side: good material cost, then the implied premium or scrap, then the premium rate.

Labor and cycle side: direct labor share, implied parts per labor hour, implied cycle time.

Production and tooling side: machine cost per part, tooling cost per part, and total cost per unit.

Important distinction for the quiz: after you calculate piece cost, you still need to sort inputs into supplier specific (things like wage rate or resin purchasing scale), part specific (like part weight), or design choice (like press size or cavities chosen for the mold).

## Plastic Parts: Beyond Piece Cost to a Sourcing Decision

Piece cost alone does not make the sourcing decision. Three more things matter:

Supplier economics: ask which cost advantage is structural (resin purchasing scale, low wage, low indirect labor, low scrap) versus which one is just a markup that could be negotiated away.

Process and tooling: a more expensive machine or tool can still produce a lower unit cost if cycle time drops enough or if more cavities increase output per cycle. Do not assume higher upfront cost means higher unit cost.

Sourcing and total cost of ownership (TCO): freight, duties, quality, capacity, and switching risk all sit outside piece cost but still matter for the final decision.

The decision question to be ready for: would you consolidate global volume with one supplier, keep two suppliers, or use a mixed strategy, and why.

## Compressors: Parametric Comparison

Compressors are the engineered subsystem case. Because the internal design is too complex to model bottoms up, the approach is a parametric (regression style) price comparison using Exhibit 3.

Functional drivers: variables that describe what the compressor does or how valuable it is (think capacity, EER or energy efficiency rating). You should have an expectation for the sign of each variable (does higher capacity push price up or down, for example).

Volume economics: annual unit volume is not a product characteristic, but it can still affect price through scale effects, so it needs to be considered even though it does not describe the compressor itself.

Regional comparison: before running any regression, compare average price, capacity, EER, and volume across regions first. Know this point cold for the quiz: raw average price alone cannot tell you which region is buying better, because the regions might be buying compressors with different specs or volumes.

Correlation: some variables may be redundant or strongly correlated with each other (for example capacity and EER might move together), and that can distort how you interpret a regression.

Model specification: the goal is a parsimonious model, meaning you include only the variables that matter and can justify leaving others out.

Managerial use: a gap between predicted price and actual price can flag a region or supplier worth investigating further, but it cannot prove on its own that someone is buying badly. It is a starting point for a conversation, not a final verdict.