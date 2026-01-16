# SAP Business One – Operational SQL Examples (Anonymised)

This repository contains **anonymised SQL examples** for SAP Business One environments.  
They are shared for **educational and practical reference**, especially for practitioners working with SAP B1 on SQL Server.

These examples illustrate how SQL can be used to support:

- inventory visibility  
- landed‑cost reference calculations  
- BOM and material‑usage analysis  
- sales and returns reconciliation  
- document‑accuracy automation (via Formatted Search)  
- general operational reporting  

All business‑specific identifiers have been removed.

---

## About These Examples

These SQL modules were originally developed for **real operational workflows** in a SAP B1 environment.  
They supported tasks such as:

- multi‑warehouse stock checks  
- cost validation  
- inbound shipment tracking  
- item‑level and container‑level operational reporting  
- reducing manual data extraction from SAP screens  

Only anonymised, non‑sensitive components are included here.  
More complex or company‑specific modules (e.g., daily stock snapshots, sales scheduling, warehouse‑level landed‑cost propagation) are **not published** due to confidentiality.

---

## Technical Context

These examples use:

- **T‑SQL** on Microsoft SQL Server  
- SAP Business One tables such as `OITM`, `OITW`, `OPCH`, `OINV`, `OWOR`, `ITT1`  
- User‑Defined Fields (UDF) and User‑Defined Tables (UDT)  
- Integration with SAP Query Manager and Formatted Search  

They are intended to be adapted to your own SAP B1 schema and business rules.

---

## Query Catalogue (Anonymised)

| File | Purpose |
|------|---------|
| `inventory_availability_by_warehouse.sql` | Multi‑warehouse stock availability (sales‑unit basis) |
| `landed_cost_moving_avg.sql` | Landed‑cost reference with 3‑period rolling average |
| `production_material_usage_by_month.sql` | 12‑month raw‑material usage for BOM items |
| `bom_parent_item_lookup.sql` | Identify parent items consuming a given component |
| `sales_and_returns_report.sql` | Unified invoice + credit memo reconciliation |
| `first_import_items_history.sql` | Identify first‑imported items for audit/traceability |
| `fs_autofill_hscode.sql` | Auto‑fill container/HS metadata in PO/AP documents |
| `duplicate_sales_order_alert.sql` | Detect potential duplicate sales orders |

These examples demonstrate practical SQL patterns for SAP B1 environments and can be adapted to a wide range of operational workflows.

---

## Disclaimer

All item codes, warehouse codes, partner identifiers, and internal business logic have been anonymised.  
These examples are provided for educational purposes and may require adaptation for production use.
