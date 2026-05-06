> Built during research for a q-commerce startup role. Demonstrates bottom-up market sizing methodology for early-stage startup contexts. Tools: Python, Pandas, Jupyter Notebook

# India Q-Commerce Market Sizing — Vegan Meat

## Problem This Solves

Founders often size markets with top-down category reports that make every opportunity look huge. The real problem is finding the narrow reachable buyer pool and the assumptions that actually drive the wedge.

## How It Helps

- Shows a bottom-up market-sizing method for a specific q-commerce category: buyer funnel, adoption filters, order frequency, AOV, and GMV scenarios.
- Separates theoretical market size from realizable platform opportunity so founders can make sharper channel and SKU decisions.
- Provides a reusable notebook, assumptions file, and output chart structure for other category-sizing projects.

## When To Fork This

- Fork this if you are sizing a niche consumer category, q-commerce wedge, D2C opportunity, or investor market memo.
- Fork it when a top-down TAM number is too broad to guide pricing, channel, or product prioritization.
- Replace the assumptions CSV, buyer funnel filters, AOV/order assumptions, and competitor table with your own market.

> "The vegan meat category on Indian quick commerce is a real but narrow opportunity — addressable GMV of ~₹627 Cr in 2024, growing to ~₹2,500 Cr by 2027. It will not become mass market. Two or three focused brands will be profitable. Most others will exit before 2027. Winning requires brutal prioritization on price, taste, and channel placement — not brand storytelling."

---

## The Core Insight

Most analysts size this market top-down using vegan food projections. That overstates it. The right entry point is the **health-motivated flexitarian** — not the ideological vegan. These are 25–35 year-old urban professionals, gym-going, protein-tracking, consciously reducing meat for health, not ethics.

---

## Key Findings

### Buyer Funnel

| Stage | Population | Filter | Rationale |
|---|---|---|---|
| Urban India Internet Users | 480M | Starting point | Urban 523M × 77% smartphone penetration *(India Briefing, 2024)* |
| Active Q-Comm Buyers | 75M | 16% | Derived from combined daily order volumes: Blinkit 6L + Zepto 3L + Instamart 5L |
| Health-Motivated (Fitness / Protein) | 22M | 29% | Conservative; 67% of India consumers report eating healthy *(Statista, 2024)* |
| Open to Plant-Based Meat | 7.5M | 34% | Consistent with global flexitarian trial data |
| **Addressable Buyer Pool (2024)** | **2.8M** | **37%** | Conservative — price barrier + limited SKU availability |

### GMV Projections (2024–2027)

| Year | Buyer Pool (M) | Avg Orders/Year | Avg Order Value (₹) | Addressable GMV (₹ Cr) |
|---|---|---|---|---|
| 2024 | 2.8 | 8 | ₹280 | **₹627 Cr** |
| 2025 | 3.9 | 9 | ₹295 | ₹1,035 Cr |
| 2026 | 5.2 | 10 | ₹315 | ₹1,638 Cr |
| 2027 | 6.8 | 11 | ₹335 | **₹2,506 Cr** |

> Note: Addressable GMV = theoretical ceiling. Realized GMV will be 30–50% lower given platform distribution challenges.

### Context

₹627 Cr sounds large. In context, India's total q-comm GMV is ~₹54,000 Cr. **Vegan meat is ~1.2% of that** — a rounding error on platform P&Ls. Platforms will carry it as a health-halo signal, not a volume driver.

---

## Competitive Landscape

| Brand | 3-Year Verdict | Key Reason |
|---|---|---|
| **Good Dot** | LIKELY WINNER | Shelf-stable, lowest price, widest distribution, profitable |
| **Wakao Foods** | POTENTIAL WINNER | Best brand equity; needs price improvement |
| Blue Tribe | HIGH RISK | Brand before product-market fit; premium price limits repeat |
| ITC Incredible | SLEEPER | Scale if prioritised; no brand identity yet |
| Imagine Meats | NICHE SURVIVOR | Foodservice-heavy, low q-comm intent |
| Beyond Meat | EXITS OR STAYS TINY | 3–5x price premium vs local alternatives |

**Winner formula:** One SKU (chicken/keema under ₹250) + taste-first positioning + Blinkit sell-through as R&D engine. Good Dot has the structural position. Wakao has the brand. The winner may be whoever combines both.

---

## Repo Structure

```
india-qcomm-market-analysis/
├── notebooks/
│   └── 01_vegan_meat_market_sizing.ipynb   # Full bottom-up analysis + visuals
├── data/
│   └── assumptions.csv                      # All input assumptions, sourced
├── outputs/
│   ├── summary_table.csv                    # GMV projections by year
│   └── market_sizing_charts.png             # Buyer funnel + GMV charts
└── README.md
```

---

## How to Run

```bash
git clone https://github.com/shubham1502-hue/india-qcomm-market-analysis
cd india-qcomm-market-analysis
pip install pandas numpy matplotlib jupyter
jupyter notebook notebooks/01_vegan_meat_market_sizing.ipynb
```

---

## Sources

| Data Point | Source |
|---|---|
| Urban internet users (480M) | India Briefing, 2024 |
| Health-conscious consumers (67%) | Statista, 2024 |
| Millennial health spending (43%) | Statista, 2024 |
| India q-comm GMV (~₹54,000 Cr) | Industry reports, 2024 |
| Platform daily orders (14L combined) | Public platform statements |
| Blinkit AOV trend (₹250→₹625) | Analyst estimates, Q2 2024 |
| India plant-based meat market ($78.6M) | IMARC, 2023 |

---

## Author

**Shubham Singh** — Founder's Office | Startup Ops  
Previously: Process Analyst at STEMpedia — built RevOps from scratch, reported directly to CEO  
📍 Bengaluru | [LinkedIn](http://linkedin.com/in/shubham9616) | [Email](mailto:shubham1502@gmail.com)
