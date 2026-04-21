# Joatham Jacob — Greentech Portfolio
### Built for comundo · April 2026

A collection of sustainability tools built to demonstrate domain knowledge in GHG accounting, CSRD reporting, and real estate carbon benchmarking — the core of what comundo does for property owners across the Nordics and Europe.

---

## What's in this repo

```
├── comundo-portfolio.html              # Main portfolio page
├── Building-emissions-benchmark-tool.html  # Project 01
├── csrd-assessment.html                # Project 02
├── CO2BenchmarkCalculator.jsx          # Project 03 (React component)
├── Portfolio_Legacy.pdf                # Supporting carbon performance report
└── README.md
```

---

## The tools

### 01 · Building Emissions Benchmark & Decarbonisation Tool
`[https://jacob-hub-esg.github.io/esgbenchmark/](https://jacob-hub-esg.github.io/esgbenchmark/)`

A four-step web application for commercial real estate carbon accounting.

**What it does:**
- Collects building type, floor area, country, and annual energy consumption by source (gas, electricity, district heating)
- Calculates Scope 1 and Scope 2 emissions using country-specific grid emission factors for 20 European countries
- Benchmarks carbon intensity against EU peer averages across six building types (Office, Residential, Retail, Industrial, Hotel, Healthcare)
- Scores CSRD readiness across six governance and data practices
- Projects a decarbonisation pathway from current intensity to net zero 2050 with 2030, 2040, and 2050 milestones

**Methodology:**
- Scope 1: Natural gas at 0.202 kg CO₂/kWh (IPCC 2006)
- Scope 2: Country grid factors ranging from Norway (0.026) to Poland (0.635), sourced from IEA / national TSO data
- District heating: 0.17 kg CO₂/kWh
- Trajectory modelled using an accelerated non-linear reduction curve

**Tech:** Vanilla HTML/CSS/JS · No dependencies · Runs fully in-browser

---

### 02 · CSRD Readiness Assessment Framework
`https://jacob-hub-esg.github.io/csrd-framework/`

A full 10-section ESRS readiness assessment covering all Environmental, Social, and Governance disclosure areas.

**What it does:**
- Walks a company through 40+ weighted yes/no questions mapped to ESRS E1–E5, S1–S4, and G1
- Calculates an overall readiness score and pillar-level scores (Environment / Social / Governance)
- Surfaces the three lowest-scoring sections as priority gaps
- Generates a tailored action plan for each section (Foundation / Intermediate / Advanced level depending on score)
- Displays a CSRD compliance timeline across the four company categories (large PIEs, large companies, listed SMEs, non-EU)

**ESRS sections covered:**

| ID | Area | Topic |
|----|------|--------|
| E1 | Environment | Climate Change |
| E2 | Environment | Pollution |
| E3 | Environment | Water & Marine Resources |
| E4 | Environment | Biodiversity & Ecosystems |
| E5 | Environment | Resource Use & Circular Economy |
| S1 | Social | Own Workforce |
| S2 | Social | Workers in Value Chain |
| S3 | Social | Affected Communities |
| S4 | Social | Consumers & End-Users |
| G1 | Governance | Business Conduct & Governance |

**Tech:** Vanilla HTML/CSS/JS · No dependencies · Runs fully in-browser

---

### 03 · CO₂ Benchmark Calculator
`https://jacob-hub-esg.github.io/my-calculator/`

A lightweight React component for instant commercial real estate carbon footprint estimation.

**What it does:**
- Accepts building type, floor area, primary energy source, building age, and occupancy rate
- Calculates total CO₂e (Scope 1+2+3), carbon intensity (kg CO₂e/m²), and energy use intensity (kWh/m²)
- Assigns a performance rating (Excellent → Poor) with a visual indicator
- Compares against five industry standards: EU Taxonomy (Paris-aligned 2030), Danish Energy Class A, BREEAM Excellent (Nordic), EU average commercial building, and EPBD regulatory minimum

**Emission factors:**
| Source | Scope 1 (kg CO₂/kWh) | Scope 2 (kg CO₂/kWh) |
|--------|----------------------|----------------------|
| DK grid electricity | — | 0.130 |
| EU avg grid electricity | — | 0.230 |
| District heating (DK) | — | 0.060 |
| Natural gas | 0.202 | — |
| Heating oil | 0.266 | — |
| On-site renewables | — | 0.020 |

**EUI baselines** sourced from IEA Commercial Buildings (2022) and CBRE Nordic Sustainability Benchmark (2023).

**Tech:** React · No external dependencies beyond React itself

---

### Supporting report · Vesterbro Retail Partners A/S
`Portfolio_Legacy.pdf`

An illustrative carbon performance report for a fictional four-property Danish retail portfolio, demonstrating how the calculation methodology translates into a real client deliverable.

Covers:
- Property portfolio overview (87,500 m² across Esbjerg, Kolding, Aarhus, Vejle)
- GHG Protocol operational control boundary
- Scope 1 & 2 results per property with intensity ratings
- Benchmark comparison against EU standards
- Stranded asset risk analysis (Vejle Storcenter)
- Data quality limitations and AMR upgrade recommendation
- Prioritised decarbonisation recommendations with CO₂ savings and post-action intensity estimates

*Status: Illustrative — dummy data for demonstration purposes.*

---

## How to run locally

No build step required for the HTML tools. Clone the repo and open the files directly in a browser:

```bash
git clone https://github.com/jacob-hub-esg
cd greentech-portfolio

# Open the portfolio page
open https://jacob-hub-esg.github.io/Comundo-portfolio/

# Or open individual tools
open https://jacob-hub-esg.github.io/esgbenchmark/
open https://jacob-hub-esg.github.io/csrd-framework/
```

For the React component (`https://jacob-hub-esg.github.io/my-calculator/`), drop it into any React project or use a sandbox like CodeSandbox / StackBlitz.

---

## Hosting (recommended)

The simplest way to share live links is GitHub Pages:

1. Push this repo to GitHub
2. Go to **Settings → Pages → Source → Deploy from branch → main / root**
3. Your tools will be live at `https://github.com/jacob-hub-esg`

Update the button links in `https://jacob-hub-esg.github.io/Comundo-portfolio/` with your live URLs before sharing.

---

## Methodology references

- GHG Protocol Corporate Accounting and Reporting Standard
- Energinet (DK grid emission factor 0.130 kg CO₂/kWh, 2023)
- EEA (EU average grid factor 0.230 kg CO₂/kWh)
- Danish Energy Agency (district heating 0.060 kg CO₂/kWh)
- IPCC 2006 Guidelines (natural gas 0.202, heating oil 0.266 kg CO₂/kWh)
- IEA Commercial Buildings Energy Data (2022)
- CBRE Nordic Sustainability Benchmark (2023)
- European Sustainability Reporting Standards (ESRS), EFRAG 2023
- EU Taxonomy Climate Delegated Act — Paris-aligned threshold 20 kg CO₂/m²/yr
- EPBD recast (2024) — regulatory minimum 90 kg CO₂/m²/yr

---

## About

**Joatham Jacob**  
MSc Environmental Change and Global Sustainability — Università degli Studi di Milano  
[linkedin.com/in/joathamjacob](https://linkedin.com/in/joathamjacob) · joathamjacob@gmail.com

Built April 2026 as part of an application to [comundo](https://www.comundo.io) — the Copenhagen-based startup automating energy data collection and carbon accounting for property owners across Europe.
