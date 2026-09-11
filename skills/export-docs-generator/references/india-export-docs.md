# India Export Documentation Standards & Layout Guide

## 1. Statutory Prerequisites for Indian Exporters
Under the Foreign Trade Policy (FTP 2023) and Customs Act, 1962, every export shipment out of India requires:
1. **IEC (Importer Exporter Code)**: 10-digit PAN-based alphanumeric code issued by DGFT.
2. **GSTIN**: 15-digit Goods & Services Tax Identification Number + 2-digit State Code.
3. **AD Code (Authorized Dealer Code)**: 14-digit bank-issued code registered on ICEGATE at the specific port of export.
4. **HSN Code (Harmonized System of Nomenclature)**: 6 or 8-digit classification code.
5. **LUT ARN**: Application Reference Number for export under Letter of Undertaking.

---

## 2. High-Risk Compliance Checks Before Document Generation

### A. SCOMET & Dual-Use Clearance Check
- Check if the product falls under Appendix 3 of Schedule 2 of ITC (HS) Classification (**SCOMET** — Special Chemicals, Organisms, Materials, Equipment & Technologies).
- Exporting SCOMET goods (e.g. specialized drones, cryptographic hardware, precision valves, biological cultures) without a specific DGFT SCOMET license is a **non-bailable criminal offense** under the WMD Act and FTDR Act.

### B. ISPM-15 Wood Packaging Quarantine Mandate
- If goods are packed on solid wooden pallets, crates, or dunnage, the wood MUST undergo **Heat Treatment (HT)** or Methyl Bromide (MB) fumigation by an accredited agency and bear the official **IPPC ISPM-15 stamp**.
- Non-compliant wood packaging leads to immediate container rejection, cargo re-export, or fumigation penalties at destination customs (often exceeding $5,000–$20,000 USD).

---

## 3. Commercial Invoice Template (India-to-Global)

```markdown
# COMMERCIAL INVOICE

**Exporter / Manufacturer:**  
ABC Exports Private Limited  
Plot No. 42, Export Promotion Industrial Park, Phase II,  
Kundli, Sonipat, Haryana - 131028, India  
**GSTIN:** 06AAAAA0000A1Z5 | **State Code:** 06 (Haryana)  
**IEC No:** 0500000000 | **PAN:** AAAAA0000A  
**LUT ARN:** AD060326001234F (Valid FY 2026-27)  
**Authorized Dealer (AD) Code:** 03001234567890 | **Bank:** HDFC Bank, New Delhi  

---

**Consignee (Buyer):**  
Nordic Home & Living BV  
Keizersgracht 421, 1016 EK Amsterdam, The Netherlands  
**VAT / EORI:** NL888888888B01 / NL888888888  

**Notify Party:** Same as Consignee  

---

| Document Detail | Value | Logistics Information | Value |
| :--- | :--- | :--- | :--- |
| **Invoice No & Date:** | EXP/2026-27/042 (11-Sep-2026) | **Port of Loading:** | Nhava Sheva (INNSA1), India |
| **Buyer's PO No & Date:** | PO-EUR-9942 (01-Sep-2026) | **Port of Discharge:** | Rotterdam Port (NLRTM), NL |
| **Country of Origin:** | India | **Final Destination:** | Amsterdam, The Netherlands |
| **Country of Destination:** | The Netherlands | **Mode of Transport:** | Ocean Freight (FCL) |
| **Incoterms® 2020:** | **CIF Rotterdam Port** | **Vessel / Voyage:** | MSC OSCAR / V.2609A |
| **Payment Terms:** | 100% Irrevocable LC at Sight | **Container / Seal No:** | MSCU7849201 / IN-884920 |

---

### Line Item Schedule

| Item No | Description of Goods | HSN Code | Qty | Unit | Unit Price (USD) | Total Amount (USD) |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: |
| 1 | 100% Organic Cotton Woven Bed Linen (King Size, 400 TC) | 6302.21.90 | 1,000 | Sets | $28.50 | $28,500.00 |
| 2 | Organic Cotton Pillow Covers (Set of 2) | 6302.31.00 | 2,000 | Sets | $6.25 | $12,500.00 |

---

### Financial Breakdown

| Component | Value (USD) | Equivalent INR (Customs Rate @ ₹86.50) |
| :--- | :---: | :---: |
| **FOB Value:** | **$41,000.00** | ₹35,46,500.00 |
| **Ocean Freight Charges:** | $2,200.00 | ₹1,90,300.00 |
| **Marine Insurance (0.25%):** | $102.50 | ₹8,866.25 |
| **Total CIF Invoice Value:** | **$43,302.50** | **₹37,45,666.25** |

**Total Amount in Words:** Forty-Three Thousand Three Hundred Two US Dollars and Fifty Cents Only.

---

### Mandatory Statutory Declarations
> *"SUPPLY MEANT FOR EXPORT UNDER BOND OR LETTER OF UNDERTAKING WITHOUT PAYMENT OF INTEGRATED TAX (IGST)"*
>
> *"We declare that this invoice shows the actual price of the goods described and that all particulars are true and correct. The goods covered by this invoice are not covered under SCOMET list or prohibited export categories."*

**For ABC Exports Private Limited**  
*(Authorized Signatory & Company Seal)*
```

---

## 4. Packing List Template (India-to-Global)

```markdown
# EXPORT PACKING LIST

**Exporter:** ABC Exports Private Limited | **GSTIN:** 06AAAAA0000A1Z5 | **IEC:** 0500000000  
**Invoice No & Date:** EXP/2026-27/042 dated 11-Sep-2026  
**Consignee:** Nordic Home & Living BV, Amsterdam, The Netherlands  
**Port of Loading:** Nhava Sheva (INNSA1) | **Port of Discharge:** Rotterdam (NLRTM)  
**Packaging Compliance:** ISPM-15 Certified Heat-Treated Euro Pallets (Stamp: IN-HT-06-881)  

---

| Package / CTN No | Marks & Numbers | Item Description | Sets / CTN | Total Sets | Net Wt / CTN (kg) | Gross Wt / CTN (kg) | Dimensions L×W×H (cm) | Total Volume (CBM) |
| :---: | :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **CTN 001 – 100** | `NHL-AMS 001/100` | Organic Cotton Bed Linen Sets | 10 | 1,000 | 14.50 | 15.80 | 60 × 40 × 35 | 8.40 |
| **CTN 101 – 150** | `NHL-AMS 101/150` | Organic Cotton Pillow Cover Sets | 40 | 2,000 | 11.20 | 12.30 | 50 × 40 × 30 | 3.00 |

---

### Summary Totals
- **Total Packages:** 150 Master Cartons on 6 ISPM-15 Heat-Treated Pallets
- **Total Net Weight:** 2,010.00 kg
- **Total Gross Weight:** 2,195.00 kg (Palletized Gross: 2,345.00 kg)
- **Total Cargo Volume:** 11.40 CBM
- **Container / Seal:** 1 × 20' FCL (MSCU7849201 / Seal No: IN-884920)

**For ABC Exports Private Limited**  
*(Authorized Signatory)*
```
