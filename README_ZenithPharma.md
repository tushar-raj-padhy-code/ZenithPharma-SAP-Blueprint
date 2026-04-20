# SAP Capstone Project — Blueprint Document
## ZenithPharma India Pvt. Ltd.

**Student:** [YOUR FULL NAME]
**Roll Number:** [YOUR ROLL NUMBER]
**Program:** SAP Integration Developer
**Batch:** 2027_SAP(OE)
**Institution:** KIIT DU
**Submission Date:** April 21, 2026

---

## 📋 Project Overview

This repository contains the Capstone Project for the SAP Integration Developer program at KIIT DU. The project is a **detailed SAP Configuration Blueprint** for a fictitious pharmaceutical manufacturing company — **ZenithPharma India Pvt. Ltd.** — covering the complete enterprise structure and customization steps across the FI, MM, and SD modules of SAP ECC 6.0 / S/4HANA.

---

## 🏭 About ZenithPharma India Pvt. Ltd.

| Field | Details |
|-------|---------|
| Company | ZenithPharma India Pvt. Ltd. |
| Industry | Pharmaceutical Manufacturing & Distribution |
| Headquarters | Hyderabad, Telangana, India |
| Plants | ZP01 — Hyderabad (Formulations), ZP02 — Ahmedabad (API & Injectables) |
| Product Lines | Tablets, Capsules, Syrups, Injectables, APIs |
| Turnover | INR 620 Crores (approx.) |
| Regulatory | GMP Certified | WHO-GMP | ISO 9001:2015 |
| Currency | INR |
| Fiscal Year | April–March (Indian FY) |
| SAP Platform | SAP ECC 6.0 (planned S/4HANA migration) |

---

## 📁 Repository Structure

```
ZenithPharma-SAP-Blueprint/
│
├── README.md                            ← This file
├── ZenithPharma_SAP_Blueprint.docx      ← Full project report (Word — editable)
└── ZenithPharma_SAP_Blueprint.pdf       ← Full project report (PDF — for submission)
```

---

## 📄 Report Contents (10 Sections)

| Section | Content |
|---------|---------|
| 1 | Project Title & Problem Statement |
| 2 | Company Profile — ZenithPharma India Pvt. Ltd. |
| 3 | FI Module — Company Code, COA, Fiscal Year, Document Types, GST |
| 4 | MM Module — Plants, Storage Locations, Batch Management, Procurement |
| 5 | SD Module — Sales Areas, Channels, DPCO Pricing, e-Invoicing |
| 6 | Cross-Module Integration — FI-MM-SD accounting flows |
| 7 | Tech Stack & Full T-Code Reference (35+ T-Codes) |
| 8 | Unique Features & Pharma-Specific Highlights |
| 9 | Future Improvements — QM, PP, S/4HANA, Serialization |
| 10 | Conclusion |

---

## 🔧 SAP Configuration Summary

### FI — Financial Accounting
- Company Code: `ZPIL` | Chart of Accounts: `ZPCA` | Fiscal Year: `ZV` (Apr–Mar)
- GST Procedure: TAXINN with HSN-level rates for pharma products
- Key T-Codes: OX02, OB29, OB62, OB37, OBC4, F110, F-28

### MM — Materials Management
- Plants: `ZP01` (Hyderabad), `ZP02` (Ahmedabad)
- Purchase Org: `ZP_PO` (Central, cross-plant)
- 9 GMP-zoned storage locations | Full batch management | Shelf-life tracking
- Key T-Codes: OX10, OX09, OX08, MM01, ME21N, MIGO, MIRO, MB56

### SD — Sales & Distribution
- Sales Org: `ZP_SO` | Channels: WS / HP / RT / EX | Divisions: FO / IN / AP / NT
- 8 Sales Areas | DPCO-compliant pricing procedure ZPRIC
- Key T-Codes: OVX5, OVX1, OVX2, VA01, VL01N, VF01, VK11

---

## 💊 Pharma-Specific Highlights

- Batch Management with shelf-life tracking and QM inspection integration (Schedule M compliance)
- DPCO Pricing Enforcement — system prevents billing above legally mandated MRP
- GMP Zone Classification for storage locations (Zones A/B/C/D — WHO-GMP aligned)
- GST HSN-level tax rates mapped per product category (Nil/5%/12%/18%)
- End-to-end batch traceability from vendor batch to production batch to customer delivery
- 4 Distribution Channels with channel-specific pricing, credit terms, and discount structures

---

## 🚀 Future Scope

- SAP QM full configuration (inspection lots, COA generation)
- GST e-Invoicing via IRP (IRN + QR code on invoices)
- SAP PP — Plan-to-Produce with Process Orders and BOM
- S/4HANA migration (Universal Journal, Fiori, Business Partner)
- SAP EWM for cold chain and temperature-controlled storage
- Drug serialization for DSCSA / EU FMD export compliance

---

*Capstone Project — KIIT DU SAP Integration Developer Program | April 2026*
