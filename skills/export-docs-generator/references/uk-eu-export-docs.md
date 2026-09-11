# UK & European Union Export Documentation Reference

## 1. Statutory Prerequisites for UK/EU Trade

### A. Economic Operators Registration and Identification (EORI)
- **UK Exporters**: Must possess a valid `GB` EORI number (e.g. `GB123456789000`) for HMRC CDS (Customs Declaration Service).
- **EU Exporters**: Must possess an EU Member State EORI number (e.g. `FR12345678900`, `DE12345678900`).
- **Northern Ireland Protocol**: Requires `XI` prefix EORI.

### B. Commodity Codes (TARIC & UK Global Tariff)
- 8-digit CN (Combined Nomenclature) code for export declarations.
- 10-digit TARIC code for import duties at destination.

---

## 2. EU/UK Statement on Origin (Rules of Origin)
Under the EU-UK Trade and Cooperation Agreement (TCA) and bilateral FTAs, exporters claiming 0% preferential tariffs must include a formal **Statement on Origin** on the commercial invoice:

```text
The exporter of the products covered by this document (Exporter Reference No: GB123456789000 / REX No: FRREX12345678) declares that, except where otherwise clearly indicated, these products are of [United Kingdom / European Union] preferential origin in accordance with the rules of origin of the Trade and Cooperation Agreement.

Place and Date: [London / Paris, 11-Sep-2026]
Name and Position of Authorized Signatory: [John Doe, Export Director]
Signature: ___________________________________
```

---

## 3. Commercial Invoice Structure (UK/EU Export Standards)

```markdown
# COMMERCIAL INVOICE / FACTURE COMMERCIALE

**Exporter:**
Apex Engineering Solutions Ltd
Industrial Park Way, Birmingham, B24 8QZ, United Kingdom
**UK VAT Reg:** GB 987 6543 21 | **EORI No:** GB987654321000

---

**Consignee (Importer of Record):**
Stuttgart Automatisierung GmbH
Industriestraße 18, 70565 Stuttgart, Germany
**DE VAT:** DE 123456789 | **EORI No:** DE123456789000

---

| Trade Field | Specification | Customs Field | Specification |
| :--- | :--- | :--- | :--- |
| **Invoice No & Date:** | UK-EXP-2026-881 (11-Sep-2026) | **Departure Point:** | Port of Dover, UK |
| **PO Reference:** | PO-STG-4410 | **Entry Customs Office:** | Port of Calais (FR000860), FR |
| **Incoterms® 2020:** | **DAP Stuttgart (Delivered at Place)** | **Transport Document:** | CMR Consignment Note #99412 |
| **Currency:** | EUR (€) | **Terms of Payment:** | Net 30 Days Bank Transfer |

---

### Goods Line Schedule

| Line | Description of Goods | TARIC / CN Code | Country of Origin | Qty | UOM | Unit Price (€) | Total Amount (€) |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | High-Precision CNC Machined Aluminium Valve Housings (Model VH-400) | 8481.90.00 | United Kingdom | 500 | Pcs | €42.00 | €21,000.00 |
| 2 | Stainless Steel Fastener Kits (M8 ISO 4017) | 7318.15.95 | United Kingdom | 1,000 | Sets | €4.50 | €4,500.00 |

---

### Totals & Value Breakdown
- **Net Goods Value (Ex-Works):** €25,500.00
- **International Freight & Transit Insurance:** €950.00
- **Total DAP Invoice Value:** **€26,450.00**
- *Note on VAT*: Zero-Rated for UK Export (VAT Notice 703). Import VAT & Destination Customs Clearance payable by Consignee under DAP terms.
```
