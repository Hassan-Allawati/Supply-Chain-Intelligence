#Project: Sohar Port Integration Audit

##Executive Summary
This audit focuses on bridging the gap between Procurement (SAP S/4HANA) and Maritime Logistics data. The goal is to identify "blind spots" in the supply chain where delayed arrivals result in unmonitored demurrage (port penalty) costs.

##Business Objectives
* **Operational Visibility:** Integrate siloed data from vendor orders and vessel tracking.
* **Risk Mitigation:** Identify high-risk vendors based on historical arrival performance.
* **Financial Control:** Calculate total value at risk from daily port penalties (OMR).

## Data Architecture (Logical View)
The audit joins three critical data layers:
1.  **Procurement:** Vendor IDs, order volumes, and purchase values.
2.  **Logistics:** Real-time vessel status and arrival reliability.
3.  **Finance:** Contractual penalty rates per day for delayed docking.
