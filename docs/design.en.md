# Game Design and Bridges to Reality

**English** | [日本語](design.md)

## 1. The Earth Twin: what it recreates

| Layer | What is modeled | Data sources (examples) |
|---|---|---|
| Nature | Climate and weather, soil, water, crop growth, fishing grounds | Weather data, satellite imagery, crop models |
| Production | Farmland, ranches, fisheries, processing plants, planting and harvests | FAO statistics, national agricultural statistics |
| Logistics | Ports, shipping lanes, roads, warehouses, the cold chain | Open port and logistics data |
| Markets | Prices, imports and exports, inventories | International prices, trade statistics |
| People | Population, age, income, diets, nutrition, disease | Census data, nutrition and health surveys |
| Environment | Greenhouse gases, water use, land-use change, biodiversity | Emissions inventories, satellite data |

- Start with a coarse map and simple models, then add detail as data and players grow.
- **No personal data.** Only public statistics and anonymous aggregates go in.

## 2. How you play

### Play a role
| Role | Decides | Struggles with |
|---|---|---|
| Farmer | What, how much and when to grow | Weather, price swings, labor shortages |
| Fisher | Where and what to catch | Depleted stocks, fuel costs |
| Logistics company | Where and how to ship, and how to keep it cold | CO2, time, spoilage |
| Store or chef | What to buy and how to sell it | Unsold stock, forecasting customers |
| Mayor or national leader | Rules, subsidies, reserves, trade | Elections, budgets, neighbors |
| Doctor or dietitian | Keeping people healthy | Lifestyle diseases, malnutrition |
| Family | What to buy, cook and eat | Budget, time, taste, health |

### Modes
- **Story:** scenarios such as "Get through a drought year that threatens 100 million people, without letting anyone starve"
- **Sandbox:** build countries and towns freely and experiment with systems
- **Co-op events:** players worldwide take on one crisis at the same time (a port blockade, a pandemic)
- **Education:** students experience how food and the planet are connected

## 3. The score: a planetary goal

```
Planetary score = healthy life expectancy + satisfaction − hunger − waste − CO2 − water and land pressure
Constraint: no country, region or role ends up worse off than at the start (Pareto improvement)
```

- Making one country rich does not raise the planetary score.
- Moves that sacrifice someone (for example, wiping out another country's farmers) violate the constraint and do not count.
- Players see **both** their own results (by country or role) and the planet's.

## 4. Discovery: human ingenuity × AI

| | Human players | AI |
|---|---|---|
| Strengths | Unexpected ideas, value judgments, cultural understanding, negotiation | Massive numbers of trials, detailed computation, fast-forwarding centuries |
| Method | Millions play, each from their own position | Learns from human strategies, then refines them through self-play (AlphaGo-style) |
| Output | New mechanisms, rules and forms of cooperation | Optimal parameters for those mechanisms, risk forecasts |

AI tests and refines the surprising moves humans find. Humans judge whether the moves AI finds would actually be accepted. The loop repeats.

## 5. Four bridges to reality

### ① Knowledge
- Good strategies are published as **open proposals**: under what conditions they work, what effect they have, and what risks they carry.
- Each comes with a reproducible scenario and data so that anyone can verify it.

### ② Pilots
- Proposals are never applied straight to a country or the world. They are first tested small, in **one town or one village**.
- With local consent, pilots measure the effect and check that no one was left worse off.

### ③ Data
- Pilot results flow back into the twin to correct the gap between game and reality.
- With each cycle, the twin's predictions get closer to reality.

### ④ Action
- Signals from the twin (where food is in surplus or short supply) become quests for real-world players.
- See [The action bridge: Hunt & Harvest](action-bridge.en.md).

## 6. Governance and funding

| Revenue | Description |
|---|---|
| Free to play | Anyone can play. No pay-to-win |
| Research and government use | Research institutions, municipalities and international organizations use it for scenario analysis |
| Business use | Logistics and food companies use it to test plans (aggregate data only) |
| Donations and funds | A share of the money saved when food waste falls |
| Education | Teaching materials for schools |

- The goal is to be governed like an **international cooperative**, owned by players, researchers, producers and municipalities.
- Rules and models are open source.

## 7. Risks and safeguards

| Risk | Safeguard |
|---|---|
| Gap between game and reality (model error) | Always run small pilots first. Show uncertainty in every prediction |
| The game becomes a political tool | Rules and data are public and verifiable. No single country or company controls it |
| A few voices dominate | Multilingual, works on low-end devices, so people of every region, age and income can take part |
| Addiction and monetization | No loot boxes. Designed so people don't overplay |
| Data misuse | No personal data. National data stays under its owners' control |
| The vulnerable get left behind | Pareto improvement is a hard constraint. Moves that leave anyone worse off do not count |
