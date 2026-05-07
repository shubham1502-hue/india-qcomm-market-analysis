# India Q-Commerce Market Sizing - Vegan Meat

Bottom-up market sizing workflow for estimating reachable q-commerce demand from funnel and assumption logic.

<!-- FOUNDER_OS_STANDARD_README -->

## The founder problem

Founders often size markets with top-down reports that make every opportunity look huge. The founder problem is finding the reachable buyer pool and the assumptions that actually drive the wedge.

## What this repo does

- documents bottom-up market-sizing logic
- uses assumptions to model buyer funnel and GMV scenarios
- exports charts and summary tables
- shows how to reason from reachable demand

## What a founder gets in 10 minutes

- assumptions CSV
- Jupyter notebook
- summary table
- market sizing chart
- methodology to reuse

## Before and after

Before:

- top-down TAM slide
- unclear adoption assumptions
- no reachable buyer logic
- weak wedge narrative

After:

- bottom-up funnel
- visible assumptions
- GMV scenario view
- clearer market entry narrative

## Who this is for

- founders exploring new markets
- strategy operators
- Founder's Office candidates
- startup generalists
- students learning market sizing

## Quick start

- Run `pip install pandas numpy matplotlib jupyter`.
- Open `notebooks/01_vegan_meat_market_sizing.ipynb`.
- Edit `data/assumptions.csv` first.
- Open `outputs/summary_table.csv` and `outputs/market_sizing_charts.png`.

## How to fork and use this for your company

1. Click Fork.
2. Rename the repo if needed.
3. Replace category assumptions in `data/assumptions.csv`.
4. Update the notebook for your market category and geography.
5. Replace source links and evidence notes.
6. Keep any private research notes out of public forks.

### Non-technical path

- Replace one CSV: `data/assumptions.csv`.
- Edit notebook text for your category.
- Run the notebook.
- Read one output first: `outputs/summary_table.csv`.

## Input format

- category assumptions
- buyer funnel steps
- adoption filters
- order frequency
- AOV
- growth scenarios
- source notes

The default sample data and examples are synthetic, anonymized, or template-only unless the repo explicitly documents a public source. Keep private customer, prospect, employee, investor, borrower, merchant, payment, or company data out of public forks.

## Output files

- `outputs/summary_table.csv`: market sizing table
- `outputs/market_sizing_charts.png`: chart output
- `notebooks/01_vegan_meat_market_sizing.ipynb`: reusable model

## Example founder workflow

- Monday: define category and wedge.
- Tuesday: collect source assumptions.
- Wednesday: run bottom-up model.
- Thursday: challenge assumptions.
- Friday: turn the result into a go/no-go or research plan.

## Customization guide

Customize these before using the repo for a real company:

- category
- geography
- buyer segments
- adoption rates
- AOV
- order frequency
- source evidence

## Where this fits in the Founder OS

This is a market strategy module. Use it when the Founder OS question is market attractiveness rather than internal operating cadence.

## Why this matters

This is not a TAM slide. It is a transparent assumption model for founder market decisions.

## Roadmap

- scenario selector
- source citation table
- Google Sheets version
- investor memo export
- multi-city model

## Contributing

Practical improvements are welcome when they make the workflow easier to fork, run, or adapt. Keep changes focused on the operating workflow and avoid adding private data or mandatory paid dependencies.

## License

MIT License. See [LICENSE](LICENSE).

## Built by

Built by Shubham Singh, a founder-facing operator focused on RevOps, GTM systems, startup metrics, AI workflows, and operating systems for early-stage teams.

## Use this in your company

Fork it, replace the sample inputs with your company context, and run the workflow. Start with the main output listed in the Quick Start section. Keep private data out of public forks.

## If you are a Founder's Office candidate

Use this repo to understand how a founder-facing operator turns messy inputs into decisions, cadence, and execution artifacts. Fork it, adapt it to a real company example, and write a short case note explaining what changed.

---

## Detailed implementation notes

The founder-facing guide above is the fastest path. The original repo-specific notes are preserved below for deeper implementation context.

> Built during research for a q-commerce startup role. Demonstrates bottom-up market sizing methodology for early-stage startup contexts. Tools: Python, Pandas, Jupyter Notebook


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

> "The vegan meat category on Indian quick commerce is a real but narrow opportunity - addressable GMV of ~₹627 Cr in 2024, growing to ~₹2,500 Cr by 2027. It will not become mass market. Two or three focused brands will be profitable. Most others will exit before 2027. Winning requires brutal prioritization on price, taste, and channel placement - not brand storytelling."

---

## Use This In Your Company

This repo is designed to be forked into an internal company workflow. Fork it, replace the sample inputs with your company context, and keep only the parts that match your operating cadence. No permission request or sales call is needed before using it; the repo is the handoff. Check the license if you plan to redistribute your version.

- Use it as a bottom-up market sizing template for category, city, channel, or wedge analysis.
- Keep the assumption stack: broad market -> reachable users -> active buyers -> addressable GMV.
- Replace q-commerce and vegan-meat assumptions with your own market, funnel, and sources.

## Minimum Edits To Make It Yours

Change these first:

| Edit | Where | Why |
|---|---|---|
| Replace market assumptions. | `data/assumptions.csv` | TAM, addressable buyers, and GMV depend on these inputs. |
| Update funnel steps and conversion logic. | `notebooks/01_vegan_meat_market_sizing.ipynb` | Makes the sizing logic fit your market category. |
| Replace source links and evidence notes. | `README.md` and notebook notes | Keeps the analysis credible for founder or investor review. |
| Regenerate summary outputs and charts. | `outputs/summary_table.csv` and `outputs/market_sizing_charts.png` | Keeps public visuals consistent with edited assumptions. |

You can leave the bottom-up sizing structure, chart layout, and output format alone on the first fork. Change assumptions first; only redesign the notebook after the sizing logic is validated.

## The Core Insight

Most analysts size this market top-down using vegan food projections. That overstates it. The right entry point is the **health-motivated flexitarian** - not the ideological vegan. These are 25-35 year-old urban professionals, gym-going, protein-tracking, consciously reducing meat for health, not ethics.

---

## Key Findings

### Buyer Funnel

| Stage | Population | Filter | Rationale |
|---|---|---|---|
| Urban India Internet Users | 480M | Starting point | Urban 523M × 77% smartphone penetration *(India Briefing, 2024)* |
| Active Q-Comm Buyers | 75M | 16% | Derived from combined daily order volumes: Blinkit 6L + Zepto 3L + Instamart 5L |
| Health-Motivated (Fitness / Protein) | 22M | 29% | Conservative; 67% of India consumers report eating healthy *(Statista, 2024)* |
| Open to Plant-Based Meat | 7.5M | 34% | Consistent with global flexitarian trial data |
| **Addressable Buyer Pool (2024)** | **2.8M** | **37%** | Conservative - price barrier + limited SKU availability |

### GMV Projections (2024-2027)

| Year | Buyer Pool (M) | Avg Orders/Year | Avg Order Value (₹) | Addressable GMV (₹ Cr) |
|---|---|---|---|---|
| 2024 | 2.8 | 8 | ₹280 | **₹627 Cr** |
| 2025 | 3.9 | 9 | ₹295 | ₹1,035 Cr |
| 2026 | 5.2 | 10 | ₹315 | ₹1,638 Cr |
| 2027 | 6.8 | 11 | ₹335 | **₹2,506 Cr** |

> Note: Addressable GMV = theoretical ceiling. Realized GMV will be 30-50% lower given platform distribution challenges.

### Context

₹627 Cr sounds large. In context, India's total q-comm GMV is ~₹54,000 Cr. **Vegan meat is ~1.2% of that** - a rounding error on platform P&Ls. Platforms will carry it as a health-halo signal, not a volume driver.

---

## Competitive Landscape

| Brand | 3-Year Verdict | Key Reason |
|---|---|---|
| **Good Dot** | LIKELY WINNER | Shelf-stable, lowest price, widest distribution, profitable |
| **Wakao Foods** | POTENTIAL WINNER | Best brand equity; needs price improvement |
| Blue Tribe | HIGH RISK | Brand before product-market fit; premium price limits repeat |
| ITC Incredible | SLEEPER | Scale if prioritised; no brand identity yet |
| Imagine Meats | NICHE SURVIVOR | Foodservice-heavy, low q-comm intent |
| Beyond Meat | EXITS OR STAYS TINY | 3-5x price premium vs local alternatives |

**Winner formula:** One SKU (chicken/keema under ₹250) + taste-first positioning + Blinkit sell-through as R&D engine. Good Dot has the structural position. Wakao has the brand. The winner may be whoever combines both.

---

## Repo Structure

```
india-qcomm-market-analysis/
├── notebooks/
│  └── 01_vegan_meat_market_sizing.ipynb  # Full bottom-up analysis + visuals
├── data/
│  └── assumptions.csv           # All input assumptions, sourced
├── outputs/
│  ├── summary_table.csv          # GMV projections by year
│  └── market_sizing_charts.png       # Buyer funnel + GMV charts
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

**Shubham Singh** - Founder's Office | Startup Ops
Previously: Process Analyst at STEMpedia - built RevOps from scratch, reported directly to CEO
 Bengaluru | [LinkedIn](http://linkedin.com/in/shubham9616) | [Email](mailto:shubham1502@gmail.com)
