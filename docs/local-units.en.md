# Starting Small: Cities, Islands, Small Nations — and the Tragedy of the Commons

**English** | [日本語](local-units.md)

**Optimize inside small, well-bounded units, and put prices and rules only at the seams between them. Then local optima stop being a tragedy and become building blocks of the global optimum.**

---

## 1. Why start with small units instead of large countries

Large countries are too complex, with too many regions, industries and institutions, to be good first test beds. We start with cities, islands and small nations.

| Unit | Strengths | Examples |
|---|---|---|
| **Islands** | Everything enters and leaves through ports and airports, so nearly all food flows can be measured. High shipping costs make waste reduction especially valuable | Japan's outlying islands, Pacific island nations |
| **Cities** | Dense populations mean many players and stores, and foot-traffic data exists | Mid-sized regional cities |
| **Small nations** | National policy itself can be piloted. Many depend on imports, so this ties directly to food security | Singapore (imports most of its food), Pacific island nations |

In Pacific island nations, growing dependence on imported processed food has gone hand in hand with some of the highest obesity rates in the world. That makes them especially meaningful places to tackle **food waste and health at the same time.**

---

## 2. What gets optimized: game × logistics × people flows

| Target | What is optimized | Example (an island) |
|---|---|---|
| **Logistics** | Ship and truck schedules, load sizes, cold-storage capacity | Ship extra before a typhoon may cancel ferries; if sailings go ahead, redistribute the surplus on the island |
| **People flows** | Movements of tourists and residents, shopping trips | Feed hotel bookings into the purchasing of hotels and restaurants to cut surplus after peak season |
| **Piggyback delivery** | Add deliveries to trips already being made | Deliver shared food along commutes, school runs and bus routes |
| **Game** | Where and when quests appear | Send rescue quests to nearby players where and when surplus appears |

---

## 3. Do local optima become a tragedy of the commons?

The **tragedy of the commons** happens when a shared resource has neither a price nor rules, so everyone acts in their own interest and the resource gets used up (Hardin, 1968).

### The tragedy happens at the seams, not across the whole

Reducing food waste is almost always **good for everyone.** When one town wastes less, it buys less from world markets, which makes food cheaper for others too (a positive externality).

But at the **seams** between units, local optimization can push costs onto others.

| Risk | What happens | Real-world parallel |
|---|---|---|
| **① Pushing waste outward** | An island imports only perfect-looking produce, so imperfect produce is thrown away at farms outside the island. Only the island's numbers improve | Losses beyond the boundary go unseen |
| **② Hoarding** | A city with better forecasting secures supplies early in a bad harvest year, leaving neighboring towns short | Export bans in the 2008 and 2022 food crises: countries protected themselves and world prices rose |
| **③ Competing for shared logistics** | One town monopolizes limited ferry slots or cold storage | Congestion of shared infrastructure |
| **④ Crowding** | Players flood places with big game rewards, causing congestion and nuisance | Crowds drawn by location-based games |
| **⑤ Shared natural resources** | Islands sharing a fishing ground each catch as much as they can | Collapse of fish stocks |

---

## 4. Five ways to fix the seams

### ① Put shadow prices only on shared resources

The root cause of the tragedy is that shared resources carry a price of zero.
Put shadow prices or caps **only** on resources shared across units (ferry slots, cold storage, fish stocks, CO2), and let each unit optimize everything else freely.

```
Each unit u:   maximize own objective − Σ (shadow price of shared resource × own use)
Coordinator:   if total use of a shared resource exceeds its cap, raise its shadow price
```

$$
\lambda_{c} \;\leftarrow\; \max\Bigl(0,\ \lambda_{c} + \alpha \bigl(\textstyle\sum_u \text{use}_{u,c} - \text{cap}_c\bigr)\Bigr)
$$

With this, **the sum of local optima matches the global optimum** (dual decomposition; see [Integrated Optimization](https://github.com/birdnnjjhiroselittle/tabemono-subete-ai/blob/main/docs/integrated-optimization.md), in Japanese).

### ② Count beyond the boundary

A unit's score counts not only waste inside it, but also **waste caused at its suppliers and destinations.** Pushing waste outward earns nothing.

```
Unit waste = waste inside + waste at suppliers caused by its orders + waste at destinations
```

### ③ Nested self-governance (Ostrom's principles)

Elinor Ostrom won the Nobel Prize in Economics for studying how communities successfully manage shared resources themselves. We apply her principles directly.

| Ostrom's principle | How it applies here |
|---|---|
| Clear boundaries | Units: islands, cities, small nations |
| Rules fit to local conditions | Each unit sets its own rules |
| Those affected help make the rules | One person, one vote for residents, stores, farmers and fishers |
| Monitoring | Waste, logistics and shared-resource use are published |
| Graduated sanctions | Pushing waste outward or hoarding: first a warning, then point deductions |
| Conflict-resolution mechanisms | A forum for units to talk things through |
| Recognized right to self-organize | No top-down orders from national governments or big companies |
| **Nested enterprises** | Unit → neighboring federation → regional federation → world, nested layer by layer |

### ④ Agreements for times of crisis

In normal times, units sign mutual-aid agreements:

- "Stockpile only up to the agreed amount"
- "Share in bad harvests and cancelled sailings"
- "Never ban exports"

This is the same idea as the disaster mutual-aid agreements between Japanese municipalities.

### ⑤ Repeated games and reputation

In a one-off deal, defecting pays; in a relationship that repeats, cooperating pays (Axelrod's research).
Make visible **how much each unit has helped its neighbors** as a reputation score, and make units with higher reputation more likely to receive help in a crisis.

---

## 5. As a game: "The Island & City League"

| Element | Description |
|---|---|
| **Teams** | Each island, city or small nation is a team; residents are the players |
| **Own score** | Waste reduction, health (vegetable intake, steps), logistics CO2 |
| **Cooperation score** | How much you helped neighbors; whether you kept shared-resource use within caps |
| **Ranking** | Own score + cooperation score. Pushing waste outward or hoarding costs points |
| **Shared events** | Typhoons closing ports, crop failures, pandemics — impossible to survive without units helping each other |
| **Practicing agreements** | Try agreements inside the game; sign the ones that work between real islands and cities (the knowledge bridge) |

### Managing people flows
- Quest rewards fall automatically when too many people gather (congestion gets a shadow price too)
- No quests in residential areas, on private property or in dangerous places
- Tourists get quests too, so visitors themselves can rescue peak-season surplus

---

## 6. Candidates for the first pilots

| Stage | Unit | Why |
|---|---|---|
| 1 | **One island** | All flows can be measured, so results are easy to see |
| 2 | **Neighboring islands** | Shared ferries and fishing grounds let us test seam problems and their fixes |
| 3 | **One regional city** | Tests people flows and game scale |
| 4 | **A small nation** | Tests national policy, imports and health policy together |
| 5 | Federations of units | Expand through nested self-governance |
