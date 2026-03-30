# 01 — Business Brief

## The Situation

Between 2021 and 2024, French food retail went through its most significant consumer behaviour shift in a generation.

Food inflation peaked at 12.8% in 2023. French households — squeezed across every budget line — responded rationally. They switched from national brands to retailer-owned private labels (MDD, *marques de distributeurs*) across almost every food category. Carrefour pasta instead of Panzani. Leclerc butter instead of Président. Intermarché canned vegetables instead of Bonduelle.

This was expected. Price shocks historically drive temporary switching. The assumption — held by most brand managers at the time — was that once inflation cooled, consumers would come back.

They have not.

---

## The Problem

By late 2024, food inflation in France had fallen below 2%. Yet private label market share has not retreated. Today, 1 in 2 products purchased in French grocery retail is a private label. National brand unit sales are down 7% since 2021. Private label unit sales are up 2% over the same period.

The switch is holding. For national brands, this is not an inflation story anymore. It is a structural problem.

Every French FMCG brand — Bonduelle, Fleury Michon, Président, Panzani, Bel — is now asking the same question:

> **Which of our categories have we permanently lost, and which can we still defend?**

Most of them do not have a clean answer. Proprietary panel data (Nielsen, Kantar) gives them aggregate market share figures, but not a causal explanation of *why* some categories held and others did not. That explanation requires going one level deeper — into the product characteristics that made certain categories more or less substitutable in the first place.

That is what this project builds.

---

## The Decision This Analysis Supports

Imagine you are the category director at a mid-sized French food company. You have a budget for brand defence — promotional spend, reformulation investment, pricing strategy adjustments. You cannot defend everything. You need to know:

1. Which categories are structurally vulnerable — where private label has embedded itself permanently because the product is functionally identical and the price gap is too large to overcome?

2. Which categories are still contestable — where national brands have a quality, nutritional, or origin-based argument that consumers might respond to if the brand makes it clearly?

3. What product-level signals predict which group a category falls into?

This analysis answers those three questions using publicly available data, economic reasoning, and transparent methodology.

---

## What We Are Not Doing

This project does not:

- Use proprietary transaction or panel data
- Make causal claims beyond what the data supports
- Prescribe specific brand strategy (that requires internal margin and distribution data we do not have)
- Pretend that public data gives us the same precision as a paid Nielsen report

We are building a rigorous, honest, reproducible analysis from public sources. The value is in the framing, the methodology, and the transparency — not in false precision.

---

## Categories in Scope

Based on where private label penetration was deepest (Kantar, INSEE, PLMA public data), we focus on the following 10 food categories:

| # | Category | French term | Why included |
|---|---|---|---|
| 1 | Pasta (dry) | Pâtes alimentaires | Highest inflation exposure, deep MDD switch |
| 2 | Butter & dairy spreads | Beurre | Large price gap, strong MDD growth |
| 3 | Cheese (everyday) | Fromages du quotidien | Highest MDD volume growth 2022–2024 |
| 4 | Canned vegetables | Légumes en conserve | Commoditised, early switching signal |
| 5 | Frozen meals | Plats cuisinés surgelés | Mixed — some differentiation possible |
| 6 | Aperitif snacks | Apéritifs / biscuits apéritif | Strong MDD growth, fragmented national brands |
| 7 | Pastry / viennoiserie | Viennoiserie industrielle | Brand differentiation unclear |
| 8 | Charcuterie | Charcuterie | National brands still strong — control case |
| 9 | Yoghurt & fresh dairy | Yaourts et laitages frais | Danone stronghold — interesting stress test |
| 10 | Cooking sauces | Sauces cuisinées | Mixed brand concentration |

---

## The Analytical Questions

### Q1 — Descriptive
Which categories experienced the largest inflationary shock between 2021 and 2024?
Which categories show the highest private label penetration today?
Are these the same categories? (They should be — but the degree matters.)

### Q2 — Analytical
Do measurable product characteristics predict category vulnerability?

Specifically, we test whether the following variables are associated with deeper, more permanent private label penetration:

- **Price premium** — How much more expensive is the national brand vs. private label in this category?
- **Nutritional differentiation** — How nutritionally different are national brand and private label products within the same category?
- **Brand concentration** — Is the category dominated by one national brand or fragmented across many?
- **Product complexity** — Do national brand products have more complex ingredient lists, quality certifications, or origin claims?

### Q3 — Strategic
Based on Q1 and Q2: which categories fall into each strategic posture?

| Posture | Signal from data |
|---|---|
| **Defend with premium** | Moderate MDD penetration + high nutritional differentiation + partial price recovery |
| **Compete on value** | Deep MDD penetration + low differentiation + large price gap |
| **Restructure** | Complete MDD dominance + no differentiation + no recovery signal |

---

## Data Sources (Summary)

| Source | What it gives us | URL |
|---|---|---|
| Open Food Facts | Product characteristics, brand vs MDD classification, nutrition, price | <a href="https://world.openfoodfacts.org/data" target="_blank">https://world.openfoodfacts.org/data</a>
|
| INSEE IPC | Monthly price indices by food category, 2015–2024 | https://www.insee.fr/fr/statistiques/series/102342213?BASIND=2342227&ZONE_GEO=2320658 |

| Kantar / PLMA (public) | Benchmark MDD market share figures by category | Public press releases and annual reports |

---

## How to Read the Rest of This Project

Each subsequent notebook builds on this brief in sequence:

- **02** — Explore each dataset before touching the analysis
- **03** — Build the category taxonomy that connects OFF and INSEE
- **04** — Measure the inflationary shock and price recovery by category
- **05** — Characterise national brand vs. MDD products using OFF
- **06** — Build the vulnerability model
- **07** — Translate findings into strategic language

Do not skip to the model. The brief and the exploration notebooks are where the thinking happens.

---

*Author: Naman Kaur — MRes Economics, Paris School of Economics*
*Project start: March 2026*