# Universal Global Export Documentation Reference (WCO Standard)

## 1. Universal Required Fields (World Customs Organization - WCO Framework)
When exporting between jurisdictions without a specialized local reference module, any standard commercial customs authority requires these baseline fields:

```
┌────────────────────────────────────────────────────────────────────────┐
│                   UNIVERSAL COMMERCIAL INVOICE HEADER                  │
├───────────────────────────────────┬────────────────────────────────────┤
│ 1. Exporter / Seller Full Address │ 5. Invoice Number, Date & Currency │
│ 2. Consignee / Buyer Full Address │ 6. Incoterms® 2020 & Named Port    │
│ 3. Notify Party (if freight)      │ 7. Payment Terms (LC, TT, DP, DA)  │
│ 4. Country of Origin & Destination│ 8. Port of Loading & Discharge     │
└───────────────────────────────────┴────────────────────────────────────┘
```

---

## 2. Standard Incoterms® 2020 Quick Reference

| Incoterm Rule | Full Name | Risk Transfers At | Cost Borne by Seller Up To |
| :--- | :--- | :--- | :--- |
| **EXW** | Ex Works | Seller's factory/warehouse | Factory floor (Buyer pays all transport) |
| **FCA** | Free Carrier | Carrier at named inland place | Delivering to buyer's nominated carrier |
| **FOB** | Free On Board | On board the vessel at port | Loading over ship's rail at origin port |
| **CFR** | Cost and Freight | On board the vessel (risk) | Ocean freight paid to destination port |
| **CIF** | Cost, Insurance & Freight | On board vessel | Freight + Minimum Marine Insurance |
| **DAP** | Delivered at Place | Ready for unloading at destination | Final delivery point (unloading by buyer) |
| **DDP** | Delivered Duty Paid | Delivered at named destination | Max seller liability: covers customs duties & taxes |

---

## 3. Universal Packing List Structure

- **Header**: Linked directly to Commercial Invoice number and date.
- **Package Hierarchy**: Pallet No $\rightarrow$ Carton No $\rightarrow$ Unit Contents.
- **Weights**: Net Weight (goods only) vs Gross Weight (goods + packaging + tare weight of pallet).
- **CBM (Cubic Metres)**: Formula = $\frac{\text{Length (cm)} \times \text{Width (cm)} \times \text{Height (cm)}}{1,000,000} \times \text{Quantity of cartons}$.
- **Container / Seal Summary**: 20' GP ($~33$ CBM / max $25$ tons), 40' GP ($~67$ CBM / max $26$ tons), 40' HC ($~76$ CBM).
