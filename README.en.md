# EARTH TABLE

**English** | [日本語](README.md)

**Build a second Earth and fail there — so that in the real one, no one has to go hungry.**

EARTH TABLE recreates the planet's food, health, logistics and environmental systems inside an open-world game. People and AI around the world play in it, discover solutions, and carry those solutions back into the real world.

> Status: concept stage (November 2026). No code yet. Ideas, feedback and collaborators are welcome.

---

## 🌍 The paradox

> The world already grows enough food for everyone. And yet:
>
> - **673 million people faced hunger** in 2024 (about 8% of humanity)
> - **More than 1 billion people** are living with obesity
> - **1.05 billion tonnes of food were wasted** in 2022 (about 19% of the food available to consumers, 60% of it in households)
> - Food loss and waste alone account for **8–10%** of global greenhouse gas emissions

**What we lack is not food, but the connections between people and food.**
Food, health, logistics and the environment are run by separate ministries, companies and countries, each with its own goals. There is no place to look at the whole system and search for moves that leave everyone better off.

EARTH TABLE builds that place — **as a game.**

---

## 🧭 Three worlds, connected

```
 ① Earth Twin (open world)
    A "second Earth" rebuilt from open data and satellites:
    climate, soil, crops, ports, shipping lanes, population,
    nutrition, prices and CO2
          │  played by people and AI worldwide
          ▼
 ② Discovery (human ingenuity × AI)
    Millions of player strategies + AI self-play (AlphaGo-style)
    → good moves for planting, logistics, policy and meals
          │  brought to reality, safest first
          ▼
 ③ Reality (pilot towns → countries → the world)
    Test good moves in real towns → feed the results back into the twin
    → the twin gets closer to reality (repeat every year)
```

---

## 🎮 The game

| Element | Description |
|---|---|
| **Roles** | Farmer, fisher, logistics company, chef, mayor, doctor or dietitian, trader, a single family… Choose any country or era |
| **Rules = real-world laws** | Crop growth, spoilage that speeds up with temperature, transport emissions, the link between nutrition and disease, and price dynamics, all modeled on science |
| **Events** | Droughts, El Niño, ports blockaded by war, pandemics, price spikes |
| **Win condition** | A planetary score: zero hunger, healthy life expectancy, CO2 and waste — under the rule that **no one ends up worse off (Pareto improvement)**. You cannot win by sacrificing someone else |
| **Cooperation first** | The planetary score only rises when players cooperate across countries and roles |

👉 Details: [docs/design.en.md](docs/design.en.md)

---

## 🌉 Four bridges from game to reality

| Bridge | What it does | Precedent |
|---|---|---|
| **① Knowledge** | Publish strategies discovered in the game as open proposals | **Foldit**: players solved, in about 10 days, the structure of a retroviral protein that had stumped scientists for years (2011) |
| **② Pilots** | Test the best strategies in real towns and villages, starting small | Local pilot programs |
| **③ Data** | Feed real-world results back into the twin so the game tracks reality | The EU's Earth digital twin, Destination Earth |
| **④ Action** | Game quests trigger real-world actions | Pokémon GO, walking-reward apps, and **"Hunt & Harvest"** |

### ④ The action bridge: "Hunt & Harvest"

Since prehistoric times, humans have been wired to enjoy searching, hunting, making and sharing. Hunt & Harvest turns those instincts into **games that rescue real food.**

| Ancient instinct | Gameplay | What happens in reality | Reward |
|---|---|---|---|
| Gathering | "Harvest spots" appear on the map | Rescue store food that would go unsold at closing time | The food itself |
| Big-game hunt | 30-player "harvest raid" | Help short-staffed farms bring in the crop | Imperfect-looking produce |
| Hunting | Rare prey | Use wild game culled for crop protection, and underused fish | Meat and fish |
| Tool making | Crafting | Cook with leftovers at home | Levels and points |
| Sharing | Delivery quests | Bring food to children's cafeterias and people in need | Community thanks, local points |

When the Earth Twin shows that a town has a surplus right now, quests go out to real players in that town. **The game world and the real world move on the same signal.**

👉 Details: [docs/action-bridge.en.md](docs/action-bridge.en.md)

---

## 🧩 The math at the core

The planetary goal is written as one equation:

```
maximize:   Σ health + Σ satisfaction − food waste − cost − CO2
subject to: safety (allergies, food poisoning), nutrition standards,
            no one worse off,
            production + stock = consumption + surplus (every food, region, day)
```

Instead of solving it centrally, we broadcast **shadow prices**, which signal where supply and demand diverge. Each country, town, store, farm and household then picks its own best move (dual decomposition).
Game rewards *are* these shadow prices, so **the game becomes a playful interface to planetary optimization.**

The full math is in the sister project [Tabemono Subete AI: Integrated Optimization](https://github.com/birdnnjjhiroselittle/tabemono-subete-ai/blob/main/docs/integrated-optimization.md) (Japanese).

---

## 🏝️ Starting small: cities, islands, small nations

Large countries are too complex, so we start with **cities, islands and small nations, whose inflows and outflows are easy to measure**, and optimize the game, logistics and people flows within each unit.

Will local optimization become a **tragedy of the commons**? Reducing waste is good for everyone. The tragedy happens at the **seams** between units: pushing waste outward, hoarding, competing for shared logistics or fishing grounds, and crowding.

- Put shadow prices or caps **only** on shared resources (ferry slots, cold storage, fishing grounds, CO2), so the sum of local optima equals the global optimum
- Count waste beyond the boundary (at suppliers and destinations)
- **Nested self-governance** based on Ostrom's principles, crisis mutual-aid agreements, reputation
- In the game, the **Island & City League**: rankings combine your own score with how much you helped your neighbors

👉 Details: [docs/local-units.en.md](docs/local-units.en.md)

---

## 🛡️ Principles

- **Neither the AI nor the game decides.** They only show options and predicted outcomes. People in each country and region decide
- **Owned by no one.** Open source, governed like an international cooperative
- **Honest about model limits.** The game is a simplified reality. Always run small pilots before acting in the real world
- **Not a propaganda tool.** Rules, data and models are public and verifiable by anyone
- **Data sovereignty.** Countries, regions and households control their own data. Only aggregates are shared
- **No addiction.** No loot boxes and no pressure to pay. Designed so people don't overplay

---

## 🪜 How the scales connect

| Scale | System | Where |
|---|---|---|
| Household | Monitoring and managing the fridge and pantry | [Tabemono Subete AI](https://github.com/birdnnjjhiroselittle/tabemono-subete-ai/blob/main/docs/home-control.md) |
| Household (AR) | AR glasses and earbuds for food waste, lost items and health | [Mimamori Kitchen](https://github.com/birdnnjjhiroselittle/mimamori-kitchen) |
| Town | Hunt & Harvest (walk, rescue, earn real food) | [docs/action-bridge.en.md](docs/action-bridge.en.md) |
| Town to world | Integrated optimization (shadow prices) | [Tabemono Subete AI](https://github.com/birdnnjjhiroselittle/tabemono-subete-ai/blob/main/docs/integrated-optimization.md) |
| **Planet** | **EARTH TABLE: discover in the game, test in reality** | Here |

---

## 🪴 Roadmap

| Stage | Description |
|---|---|
| 0 | Publish the concept and gather collaborators (researchers, game developers, farmers, logistics, healthcare, government) |
| 1 | Small twin: a simple game of one island's or city's food flows, plus a Hunt & Harvest pilot |
| 1.5 | Island & City League: connect neighboring islands and cities to test seam problems (pushing waste outward, hoarding, shared resources) and their fixes, then move on to a small nation |
| 2 | National twin: recreate one country from public statistics, weather and logistics data. Players and AI search for strategies |
| 3 | Earth Twin: recreate the world from FAO and satellite data, with an international player community |
| 4 | Test game-discovered strategies in pilots around the world and feed the results back into the twin |

## 📚 Documents

- [Game design and bridges to reality](docs/design.en.md)
- [The action bridge: Hunt & Harvest](docs/action-bridge.en.md)
- [Starting small: cities, islands, small nations — and the tragedy of the commons](docs/local-units.en.md)
- [Sources](docs/sources.md)

## License

[MIT](LICENSE)
