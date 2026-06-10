# 🌿 Supply Chain Decarbonisation — Scope 3 Carbon Accounting Model

A portfolio project demonstrating end-to-end GHG Protocol Scope 3 carbon accounting and supplier engagement strategy for a fictional mid-sized apparel brand, **Norvik Apparel GmbH** (Hamburg, Germany).

Built to showcase applied sustainability consulting skills for corporate roles in the DACH region.

---

## 📋 Project Overview

| Item | Detail |
|------|--------|
| **Company** | Norvik Apparel GmbH (fictional) |
| **Industry** | Mid-market apparel — organic cotton, recycled polyester, Merino wool |
| **Revenue** | €85 million |
| **Scope** | GHG Protocol Scope 3 — Category 1 & Category 4 |
| **Base Year** | 2024 |
| **Target** | −30% absolute Scope 3 emissions by 2030 |
| **Framework** | SBTi near-term target + SBTi FLAG (land-use emissions) |

---

## 📁 Repository Contents

```
├── norvik_scope3_model.xlsx              # Full carbon accounting model (5 sheets)
└── norvik_supplier_engagement_strategy.docx  # 3-section supplier engagement strategy
```

---

## 📊 The Carbon Accounting Model (`norvik_scope3_model.xlsx`)

A fully formula-driven Excel model with five sheets:

### Sheet Structure

| Sheet | Purpose |
|-------|---------|
| 📋 README | Model overview, colour conventions, step-by-step instructions |
| ⚙️ Assumptions | All emission factors, spend data, and target parameters — single source of truth |
| 🚢 Cat4 Transport | Category 4 upstream transport emissions per supplier |
| 🌾 Cat1 Materials | Category 1 purchased goods emissions — physical intensity + spend-based cross-check |
| 📊 Dashboard | Aggregated Scope 3 results, supplier tier table, hotspot analysis, 2030 tracker |

### Supplier Data (7 global suppliers)

| Supplier | Location | Material | tCO₂e | % Share | Tier |
|----------|----------|----------|-------|---------|------|
| Textil Maroc SA | Morocco | Knitted wool garments | 2,014 | 44.2% | A |
| PT Garuda Tekstil | Indonesia | Cut & sewn T-shirts | 886 | 19.5% | B |
| Nordic Wool AS | Norway | Raw Merino wool | 669 | 14.7% | B |
| Chennai Dye Works | India | Dyed & finished fabric | 395 | 8.7% | B |
| Shanxi Cotton Co. | China | Organic cotton yarn | 331 | 7.3% | C |
| Far East Poly Ltd. | Vietnam | Recycled polyester fabric | 203 | 4.5% | C |
| EcoZip Taiwan | Taiwan | Recycled nylon zips | 56 | 1.2% | C |

**Total Scope 3: 4,553.10 tCO₂e | 2030 Target: 3,187.17 tCO₂e**

### Methodology

- **Category 4:** `Volume (kg) ÷ 1,000 × Distance (km) × Emission Factor (kgCO₂e/tonne-km)`
- **Category 1 (primary):** `Volume (kg) × Material EF (kgCO₂e/kg)` — physical intensity method
- **Category 1 (cross-check):** `Spend (€) × Sector EF (kgCO₂e/€)` — spend-based method

### Emission Factor Sources

| Source | Used For |
|--------|---------|
| DEFRA 2024 | Transport emission factors (all modes) |
| SAC Higg MSI 2023 | Wool and cotton material emission factors |
| Textile Exchange 2023 | Recycled polyester and nylon emission factors |
| ecoinvent 3.9 | Cut & sew manufacturing energy intensity |
| EXIOBASE | Spend-based sector emission factors (cross-check) |

> **Limitation note:** All material emission factors use Tier 2/3 data (industry averages). Primary data from supplier energy bills would be required for a Tier 1 calculation under the GHG Protocol hierarchy.

---

## 📄 Supplier Engagement Strategy (`norvik_supplier_engagement_strategy.docx`)

A 3-section professional strategy document outlining how Norvik will engage its supply chain to achieve the 2030 target.

### Document Structure

**Section 1 — Context & Baseline**
- CSRD regulatory driver and SBTi FLAG commitment
- Emissions baseline: 4,553.10 tCO₂e, 97.5% in Category 1
- Top 3 emitters and hotspot analysis
- 30% absolute reduction target aligned to Paris Agreement

**Section 2 — Tiered Engagement Model**
- **Tier A** (>30% Scope 3): Textil Maroc SA — CDP disclosure, joint roadmap, co-investment, contract termination if non-compliant
- **Tier B** (10–30%): PT Garuda Tekstil, Nordic Wool AS, Chennai Dye Works — GHG tools, training, 2-year improvement plan
- **Tier C** (<10%): Shanxi Cotton Co., Far East Poly Ltd., EcoZip Taiwan — annual self-assessment, escalation triggers

**Section 3 — Incentive Mechanisms & Governance**
- Commercial incentives: preferred supplier status, volume guarantees, verified green premium
- Capacity building: funded training cohort, GHG Protocol tool access, co-funded Tier A audits
- Escalation & exit: red flag criteria, 6-month remediation window, 2028 contract performance clause
- Governance: Supplier Sustainability Working Group, quarterly internal review, annual GRI 308 disclosure

---

## 🔑 Key Insights

1. **Category 1 dominates at 97.5%** — transport optimisation alone cannot meet the 2030 target; material substitution is the primary lever
2. **Proximity ≠ low emissions** — Textil Maroc SA is the closest major supplier yet accounts for 44% of total Scope 3, driven entirely by Merino wool's land-use footprint (18.5 kgCO₂e/kg)
3. **Biggest quick win** — EcoZip Taiwan accounts for only 1.2% of Scope 3 but uses air freight; switching to sea freight saves ~21 tCO₂e at near-zero cost
4. **FLAG commitment matters** — two suppliers (Textil Maroc SA, Nordic Wool AS) have emissions driven by livestock methane and agricultural land use, which fall outside standard SBTi energy targets and require the FLAG framework

---

## 🛠️ Tools & Frameworks Used

- GHG Protocol Corporate Value Chain (Scope 3) Standard
- SBTi Near-Term Target Setting Criteria
- SBTi FLAG Guidance (v1.0, 2022)
- DEFRA 2024 Greenhouse Gas Conversion Factors
- SAC Higg Materials Sustainability Index
- Textile Exchange Preferred Fiber & Materials Report 2023
- GRI Standard 308 (Supplier Environmental Assessment)
- CDP Supply Chain Programme
- Microsoft Excel (formula-driven model, no macros)
- Microsoft Word

---

## 📌 Disclaimer

Norvik Apparel GmbH is a fictional company created for portfolio demonstration purposes. All supplier names, financial figures, and emissions data are simulated. Emission factors are sourced from publicly available databases and are cited throughout the model.
