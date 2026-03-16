#  Strategic Maritime & Procurement Risk Audit

### **Sohar Port Operations | Multi-Dataset Supply Chain Analysis**

##  Executive Summary

This project represents a comprehensive audit conducted to identify financial exposure within our procurement pipeline. By integrating **internal procurement data** with **UNCTAD global maritime benchmarks**, I identified significant capital-at-risk tied to high-congestion shipping lanes. This analysis provides actionable insights for vendor diversification and lead-time optimization.

---

##  Key Audit Findings

The following table summarizes the high-risk suppliers identified by joining internal spend data with external port performance metrics.

| Supplier | Home Country | Value At Risk (Processing) | Port Wait Time (Days) | Risk Level |
| --- | --- | --- | --- | --- |
| **Gamma_Co** | Russian Federation | **$1,875,200.00** | **1.60** |  CRITICAL |
| **Beta_Supplies** | Germany | $450,300.00 | 0.95 |  MEDIUM |
| **Alpha_Inc** | Singapore | $120,000.00 | 0.46 |  LOW |

> **Strategic Insight:** **Gamma_Co** represents our primary vulnerability. The combination of nearly $1.9M in pending value and the highest regional port delays suggests an immediate need for contingency planning or alternative routing.

---

##  Project Structure

To ensure transparency and reproducibility, the repository is organized as follows:

* **[ Datasets][(https://www.google.com/search?q=./Datasets](https://github.com/LSCM-Student/Maritime-Port-Performance-Project-/tree/main/Datasets)):** Contains raw CSV files for Procurement KPIs and Maritime Port Performance.
* **[ SQL Queries][(https://www.google.com/search?q=./](https://github.com/LSCM-Student/Maritime-Port-Performance-Project-/tree/main/SQL_Queries):** Contains structured logic used in Google BigQuery to clean and join the datasets.

---

##  Technical Audit Workflow

### **1. Internal Performance Overview**

* **Objective 1: Value at Risk (VAR):** Calculated the total financial value of all shipments currently in "Processing" status to identify capital frozen in the supply chain.
* **Objective 2: Lead-Time Audit:** Benchmarks the average days elapsed between order date and delivery to identify underperforming vendors.

### **2. External Benchmarking**

* **Objective 3: Maritime Performance:** Analyzed the **UNCTAD Maritime Port Performance** dataset, specifically filtering for **'Container ships'** during the **'2023-S2'** period to identify global bottleneck regions.

### **3. Strategic Risk Mapping**

* **Objective 4: Logic Mapping:** Created a **Common Table Expression (CTE)** to bridge internal supplier names with external economy labels. This allowed for a direct correlation between internal spending and external infrastructure delays.

---

## Business Recommendations

Based on the SQL output, I recommend the following C-Suite actions:

1. **Risk Mitigation:** Reduce order volume with **Gamma_Co** by 15% until regional port wait times drop below 1.2 days.
2. **Lead-Time Optimization:** Shift high-priority container shipments toward **Alpha_Inc** (Singapore), leveraging their superior port turnaround efficiency.
3. **Data Integration:** Automate this SQL pipeline to provide real-time risk alerts for the Procurement team.

---

