<div align="center">

# 🌐 Trade Agent Skills (`trade-agent-skills`)

### The Missing Cross-Border Trade & Export Compliance Skills for Claude Code, Antigravity, & AI Agents

[![GitHub Stars](https://img.shields.io/github/stars/Om-Talaviya/claude-trade-skills?style=for-the-badge&logo=github&color=FFB800)](https://github.com/Om-Talaviya/claude-trade-skills/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Claude Code Plugin](https://img.shields.io/badge/Claude%20Code-Plugin%20Ready-6B46C1?style=for-the-badge&logo=anthropic)](https://claude.ai)
[![Antigravity Compatible](https://img.shields.io/badge/Antigravity-Verified-00C49F?style=for-the-badge)](https://github.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen.svg?style=for-the-badge)](https://github.com/Om-Talaviya/claude-trade-skills/pulls)

<p align="center">
  <b>Eliminate US-centric customs bias in AI.</b><br/>
  Generate country-accurate export paperwork (India, UK/EU, UAE/GCC, Global) and automate Indian GST export mechanics (LUT, ICEGATE Shipping Bill Refunds, GSTR-1/3B Reconciliation, and RFD-01).
</p>

[Quickstart](#-quickstart) •
[Why This Exists](#-the-problem-this-solves) •
[Included Skills](#-included-skills) •
[Interactive Examples](#-sample-generated-artifacts) •
[Contributing](#-contributing)

</div>

---

## ⚡ The Problem This Solves

Almost every existing AI tool, prompt, and skill repository defaults exclusively to **US Customs and Border Protection (CBP)** rules (EIN, 19 CFR, US HTS 10-digit codes).

When cross-border businesses, freight forwarders, or developers try to generate compliant export documentation or navigate tax incentives outside the US, AI models either hallucinate non-existent forms or fail on mandatory origin compliance:

```
┌───────────────────────────────────────┬────────────────────────────────────────┐
│ ❌ Generic AI & Existing Tools        │ ✅ Trade Agent Skills Suite            │
├───────────────────────────────────────┼────────────────────────────────────────┤
│ • Defaults to US EIN & CBP formatting │ • Country-accurate Tax IDs (IEC, GSTIN,│
│                                       │   EORI, VAT, TRN)                      │
│ • Hallucinates US sales tax on export │ • Implements Section 16 Zero-Rated     │
│                                       │   Supply & Rule 96A LUT mechanics      │
│ • No concept of ICEGATE / Shipping    │ • Error diagnostics for SB001–SB006    │
│   Bill automated IGST refunds         │   Customs EDI transmission issues      │
│ • Produces vague invoice templates    │ • Incoterms® 2020 breakdowns, ISPM-15   │
│   unusable for customs clearance      │   packing lists, & origin declarations │
└───────────────────────────────────────┴────────────────────────────────────────┘
```

---

## 📦 Included Skills

```
skills/
├── gst-export-compliance/        # 🇮🇳 India GST Export Mechanics & Refunds
│   ├── references/
│   │   ├── lut-filing.md          # Form RFD-11 guide, eligibility, timelines
│   │   ├── igst-refund-icegate.md # Rule 96(10) bar, Table 6A, SB001-SB006 errors
│   │   ├── gstr-reconciliation.md # 3-way match: GSTR-1 vs GSTR-3B vs Customs EDI
│   │   ├── rfd01-lut-refund.md    # Rule 89(4) unutilized ITC refund formula & Statement 3A
│   │   ├── export-services-compliance.md # 5 tests of Sec 2(6), Intermediary tax defense
│   │   └── fema-edpms-compliance.md      # RBI 9-month realization, Rule 96B refund clawback
│   └── SKILL.md
│
└── export-docs-generator/        # 🌍 Global Multi-Region Shipping Documentation
    ├── references/
    │   ├── india-export-docs.md   # IEC, GSTIN, HSN, SCOMET checks, ISPM-15 packaging
    │   ├── uk-eu-export-docs.md   # GB/EU EORI, VAT, TARIC CN codes, Origin Statements
    │   ├── uae-gcc-export-docs.md # TRN, Dubai Customs Mirsal 2, bilingual layouts
    │   └── generic-export-docs.md # Universal WCO commercial invoices & packing lists
    └── SKILL.md
```

### 1. `gst-export-compliance`
- **Zero-Rated Supply Routing**: Automatically determines whether an exporter should use **Option A (LUT + ITC Refund)** or **Option B (IGST Paid + Automated ICEGATE Refund)** based on working capital and cash-flow preferences.
- **ICEGATE Error Resolution**: Built-in resolution playbook for customs refund freezes (**SB001** EGM missing, **SB003** GSTIN mismatch, **SB005** invoice/port mismatch).
- **Rule 89(4) Computation**: Formulates the exact statutory maximum refund calculation for Form GST RFD-01:
  $$\text{Refund Amount} = \frac{\text{Turnover of Zero-Rated Supply} \times \text{Net ITC}}{\text{Adjusted Total Turnover}}$$

### 2. `export-docs-generator`
- **Country-Accurate Invoices**: Inserts statutory exporter identifiers (India IEC/GSTIN, UK/EU EORI/VAT, UAE TRN) and mandatory zero-rate endorsement clauses.
- **Incoterms® 2020 Math**: Automatically splits FOB value, international freight, and marine transit insurance to compute exact CIF/CIP values.
- **ISPM-15 Packing Lists**: Calculates carton packaging, tare weight, palletization metrics, and cubic volume (CBM).

---

## 🚀 Quickstart

### Option A: Install in Claude Code (One-Liner)

```bash
# Direct marketplace installation
/plugin marketplace add Om-Talaviya/claude-trade-skills
```

Or clone directly into your Claude skills directory:
```bash
git clone https://github.com/Om-Talaviya/claude-trade-skills.git ~/.claude/plugins/claude-trade-skills
```

### Option B: Use with Antigravity IDE & Cursor

Clone or copy the `skills/` directory into your project's `.agents/skills/` or global `~/.gemini/config/skills/` directory:

```bash
mkdir -p .agents/skills
cp -r skills/* .agents/skills/
```

---

## 💡 Real-World Prompts You Can Try

Once installed, simply chat with your AI agent naturally:

```markdown
> "I am exporting $40,000 worth of brass handicrafts from Moradabad, India to London, UK under CIF terms. Generate a fully compliant commercial invoice and packing list under LUT."

> "My IGST refund of ₹3.5 Lakhs is stuck on ICEGATE with error code SB005. How do I fix this in my next GSTR-1 filing?"

> "Draft a Statement on Origin and commercial invoice for exporting CNC aluminum parts from Birmingham, UK to Stuttgart, Germany under DAP Incoterms."
```

---

## 📋 Sample Generated Artifacts

<details>
<summary><b>🔍 Click to preview sample Commercial Invoice (India to Netherlands)</b></summary>

```markdown
# COMMERCIAL INVOICE

**Exporter / Manufacturer:**  
ABC Exports Private Limited  
Plot No. 42, Export Promotion Industrial Park, Phase II, Kundli, Haryana - 131028, India  
**GSTIN:** 06AAAAA0000A1Z5 | **IEC No:** 0500000000 | **LUT ARN:** AD060326001234F  

**Consignee:** Nordic Home & Living BV, Keizersgracht 421, Amsterdam, The Netherlands  
**Incoterms® 2020:** CIF Rotterdam Port | **Port of Loading:** Nhava Sheva (INNSA1)  

| Item No | Description of Goods | HSN Code | Qty | Unit | Unit Price | Total Amount (USD) |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: |
| 1 | 100% Organic Cotton Woven Bed Linen | 6302.21.90 | 1,000 | Sets | $28.50 | $28,500.00 |
| 2 | Organic Cotton Pillow Covers (Set of 2) | 6302.31.00 | 2,000 | Sets | $6.25 | $12,500.00 |

**FOB Value:** $41,000.00 | **Ocean Freight:** $2,200.00 | **Marine Insurance:** $102.50  
**Total CIF Invoice Value:** **$43,302.50 USD**

*Declaration: SUPPLY MEANT FOR EXPORT UNDER BOND OR LETTER OF UNDERTAKING WITHOUT PAYMENT OF INTEGRATED TAX (IGST)*
```

See the full sample in [examples/india-lut-invoice-sample.md](examples/india-lut-invoice-sample.md).
</details>

---

## 🧪 Evals & Verification

This repository includes a benchmark evaluation suite in [evals/eval-test-cases.json](evals/eval-test-cases.json) to test accuracy across:
- Correct statutory endorsement verification
- ICEGATE error diagnostic precision
- Multi-currency Incoterms freight/insurance separation

---

## 🤝 Contributing

Contributions of new country reference files (e.g., Japan, Singapore, Brazil, Australia) are warmly welcomed! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for details on submitting pull requests.

---

## ⚖️ Disclaimer & License

*This repository provides preparation, formatting, and computational tools for AI coding agents. It does not file documents automatically or substitute for professional advice from a licensed Customs Broker (CHA), Freight Forwarder, or Chartered Accountant (CA).*

Released under the [MIT License](LICENSE).

---

<div align="center">
  <b>⭐ Star this repo if you find it useful for international trade & AI agent development! ⭐</b>
</div>
